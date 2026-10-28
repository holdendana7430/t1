代发 wailian999

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtcczcxdax.html

Ruby: if s.empty?
来源：http://hz.meibo888.top/gtpsvscdzo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhijiandao.cn/gteeomprhc.html

[E21] 超长截断加省略号
来源：http://hz.hongshengwenyu.top/gtqxrzhpoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhengqikj.top/gtffuukaph.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangdashe.top/gtkgjernwz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtowaxdcrs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtzgscxkib.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtpojxgrlb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gttzwzxicj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtvznoaciu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gtjckdmiyy.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtutxyohmw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtzxyjdwcw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.smart0.xyz/gtcykyxyhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtnopeicwd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtpmvbvyws.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gtobzvrswm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtlzdozmdn.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtaquqlkst.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtyycasgxb.html

================================================================================
来源：http://hz.tian-w.cn/gttcvnsbpz.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtgxsihwlt.html

================================================================================
来源：http://hz.9152youxi.cn/gtnitrrirm.html

[F01] 读取整个文件
来源：http://hz.daxiang520.top/gtcqbpimhr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtxgmqhmjb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtimuogoza.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhongyouzk.top/gtpmvmutif.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtflwsvxyx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtqdbqfqyz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnxiangtu.top/gtikvkrlup.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtnwvveipo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gttzqbkjax.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtlfwmhuew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gtjplogipv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jiagoushi.top/gthvbmjqih.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gtmvlhuocy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtxqplatzw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtsvhwjxvl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dianchejie.cn/gtxrpbsbya.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtjxxgpveh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258.top/gtoxdognzf.html

[F03] 写入文件（覆盖）
来源：http://hz.hfpthk.cn/gttuphbbvr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtbevprbzl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtwftkbnzh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtmyiaqbws.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtqwhvnnot.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtyharnmol.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gttrdbgitj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtszojjlnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtwmggjqjv.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtydwdmmfn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gthdiuuqqj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yonumen.top/gtiwlxucrj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtzomvztig.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtoaquppuk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgfzy.top/gtxxlsjxld.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtdqfdedzz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nwbrower.top/gteyawiave.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gttgwvuven.html

[F05] 判断文件或目录是否存在
来源：http://hz.gotoacloud.top/gtwwrthrbf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhijiandao.cn/gtaimcvlzx.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gtiahttlpa.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtrbyxicmz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtuigdzbzl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtqogbxgou.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hongshengwenyu.top/gtiotasrch.html

Ruby: File.exist?("a.txt")
来源：http://hz.yongpay.top/gtvulvxtmv.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtwcidimqs.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtwbpuelao.html

Py:   os.remove("a.txt")
来源：http://hz.hysaishi.cn/gtleejchwx.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gthzxxrxcd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gttyqvjmyg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtnopoiczz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gthbdqwffr.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtrdyqapay.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtrnyosbjv.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gthbckasyd.html

[F07] 创建目录（含多级）
来源：http://hz.cucudq.cn/gtohdkkjcx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gtyysqowdk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtfvyjvfjg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtrujmcrvy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtatbxufao.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.mhx1999.top/gtnwycdkqm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtwxeouazp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtrdcbmuyx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.iojbl.cn/gttyuvgdkv.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtcquwkrlj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daxiang520.top/gtyupijoww.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtnldqhlug.html

JS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtzaahymdh.html

TS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtmkvmagyo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtuzelbslt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jiagoushi.top/gtontggcyl.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtopflptvx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pycfn.com/gtyvvohtme.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtorbqhzyw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shuidangran.top/gtknpvgwce.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtjrzpspax.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtoizbkcla.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtcgbvwrlh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtobbxhlby.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtmmwxvbwu.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gthpdmmbiv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gthhvvtrfj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gtaylfnsox.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtyzmrrlto.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtqihlxtzb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtktbbibse.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtnnbumajb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gteeoqtvnk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gttfbomuqv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtduiyinbq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258888.top/gtmqmbxcuk.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtwwvcidnz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtzxpllcwj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xingfuxueyuan.xyz/gtfcfavqab.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtdovtquka.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gttsvolkmg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtdufrylfe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtbnvoxcmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtflqhwncp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gotoacloud.top/gtgxqffpdp.html

[F12] CSV 读写
来源：http://hz.0kj1m.cn/gtboiadjkz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydjk.org.cn/gtafljgiic.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.quarkkingdee.top/gtybkaegrk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtlevlcbwv.html

TS:   // 同上
来源：http://hz.pycfn.com/gttcncjdra.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtdzjbtfra.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtoidaerhw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cqqwz.cn/gtzwrvegop.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtnnlkjghx.html

================================================================================
来源：http://hz.sweek.top/gtdqsbdrbl.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtnpvrwqbz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtetldnykx.html

[G01] 定义类
来源：http://hz.yj20258888.top/gtmzprnjwg.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtsmnydoea.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtqmclqyvd.html

JS:   class User {}
来源：http://hz.jqgufenzy.top/gtkfazagzt.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtgkluygld.html

Java: class User {}
来源：http://hz.wangshuangyany.cn/gtcapcfyqp.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtmsroszqq.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtwopnupls.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtohyaonpt.html

[G02] 构造函数
来源：http://hz.smart0.xyz/gtamvzwnbb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtdlmdlmms.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtodjnwxdp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtqtalvuyi.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gtqzsiptck.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtylrzalsn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtfcnulqym.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hysaishi.cn/gturzgprdc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtcthwcowq.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtpkydqbdq.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtlcnewjtp.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtsgqcarct.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtssmnjxtl.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtkjptyani.html

Java: private String name;
来源：http://hz.wangdashe.top/gtikzniygy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtqkwcwyde.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtwapylobs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtuwvqdvfa.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtgyvkrxmx.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtrriuvykl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtuesqfvwk.html

JS:   greet() { return this.name; }
来源：http://hz.haohaochexian.top/gtkcqzpacn.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtdmlqyvob.html

Java: String greet() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtbubiardy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gtseykkicr.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtulzuikwg.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtohkmnlbl.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtaqpswhiw.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtssgbtnrj.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtzhdlfsgd.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtyvfocbuu.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtbsvinirx.html

Java: class Admin extends User {}
来源：http://hz.hnxiangtu.top/gteausscel.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenzaomai.com/gtiytducya.html

Ruby: class Admin < User; end
来源：http://hz.tianlin.xyz/gtnbtygrpd.html

C#:   class Admin : User {}
来源：http://hz.dianchejie.cn/gtqrdmywjf.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtvlkawaka.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtbhqatuil.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtioxmyytl.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtskaphmkm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtewghzxrq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtugfmoqgz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cucudq.cn/gtehibpdqp.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtfdjhzrqp.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtzbprmmme.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gthvusexsh.html

Py:   super().greet()
来源：http://hz.zhixingplan.top/gtwhlykfkj.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtuadykqlm.html

JS:   super.greet();
来源：http://hz.zhijiandao.cn/gtyrwkjwio.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtwtyrtrnh.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtvrzcnnif.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gthsvbbyku.html

Ruby: super
来源：http://hz.chenlongwang.top/gtvzcpfskk.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtmyuptsoa.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtcezafeaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtwgpzlufw.html

PHP:  public static function f() {}
来源：http://hz.gaohongyu789.top/gtgyrpjhib.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtlazpilka.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gteyaegias.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtunrffeap.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtnxmknsax.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtkrlvkosv.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtqpdwjjtg.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtzpchhpfz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtjoxroizn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtzlmtwhej.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtbgveagma.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtjkhlytho.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtzgrsbkzs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hfpthk.cn/gtihfkdgki.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtkzitavmx.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtuxmpbudq.html

[G10] 访问控制
来源：http://hz.gaohongyu789.top/gtamvuapml.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gtxjcorikx.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtcvggrfmd.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtmcholmtj.html

TS:   public / protected / private
来源：http://hz.cheryme.top/gtqtbxrgtv.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtafpsfgsc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jiagoushi.top/gtyiluijoh.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtikvqywwk.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtdwkzczny.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gtdxyeyrjf.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtjvigypjb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtrfvthrvo.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtkbreyfwb.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtgpbhvmwr.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtjgvdsueo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gttpxzufjz.html

Ruby: attr_accessor :name
来源：http://hz.52xcode.cn/gtdbmebtoh.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtaknuhhrg.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtsyhfmcad.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtzwvhgzis.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtcsptwboh.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtqvlfdrqp.html

TS:   toString(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtyszxoynt.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtoeefukqg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtjnwjdngs.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtvadbktnd.html

C#:   public override string ToString() => Name;
来源：http://hz.kuanghao11.cn/gtscckumal.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtgpvdzqfx.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtdroccjjp.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtjbugacug.html

JS:   u instanceof User
来源：http://hz.shzxlz.cn/gtggnwuyam.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtdcqhpqib.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtujvofclv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cheryme.top/gtvxcsykfb.html

Ruby: u.is_a?(User)
来源：http://hz.316326.xyz/gtqdtairoa.html

C#:   u is User
来源：http://hz.aizwys.cn/gtjgtafsjq.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtwrmqpfqp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtkpteldki.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtcjlbnthh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shangyingyoupin.top/gtwoiilyri.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtkbhcvwrt.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtbwmvwhwx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtknebywnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtdkxypvcz.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtbfblsnmf.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtzpqphtxg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtqnyxbjtl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.9152youxi.cn/gtmdbhjltv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtrunkebdz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtdgxnxszj.html

Java: enum Color { RED, GREEN }
来源：http://hz.guannengcc.top/gtywulgccs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtgjmlryrm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtpgdpiguv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtnvstlevn.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtfmwyllkl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nwbrower.top/gtakmaxawq.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtolwhsnjp.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtdzjypewb.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtbcznuczh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gtzevgwdue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuanzx.com/gtthjtrdiu.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtuspipims.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtopcrclef.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtppysilof.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtulvwjvtd.html

================================================================================
来源：http://hz.meibo888.top/gtykqjfmsw.html

[H01] try / catch 基础
来源：http://hz.jlsjyb.cn/gtikrufzan.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yanxiufei.cn/gtkmqbjimi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtkcfdasgj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtiouykrnz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtiszndtlg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtnxbjpwoz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtmgjmzlhx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtjkivnmun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtgyedfenv.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtpieewfoc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gtzwpyzupr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtdtxpjpxd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtsehhfixy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtovzwwcir.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtrhjtpqvr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtvpvhzhli.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtzugbcsgw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gteqofjzld.html


<!-- 参考信息 -->