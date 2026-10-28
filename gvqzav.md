代发 wailian999

Ruby: s.lines
来源：http://hz.yuxming.cn/gtfwpeymcq.html

C#:   s.Split('\n')
来源：http://hz.hammf.cn/gtyzqeumjz.html

[E20] 判断字符串是否为空
来源：http://hz.nanxuanxn.top/gtvwmigahi.html

Py:   if not s:
来源：http://hz.cdnleiting.top/gtudlojarz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.bjfxy.top/gtyhvmkumc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.andypj.xyz/gtqcyuhowp.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtnttqppxr.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtlbaajbqg.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtqzylyduc.html

Ruby: if s.empty?
来源：http://hz.havefunace.top/gtxbgsuccz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtsswufwyp.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtkhkqwojt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtuvxdaibz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtsphkmnep.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtqvurzivt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtcgdppsja.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtvhvwrgzq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pengpengdd.cyou/gtliptqfwm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fzhhl.top/gtpiwjduqu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gthupxpqhu.html

[E22] 字节长度与字符长度
来源：http://hz.hfpthk.cn/gtlostnipp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.havefunace.top/gtphyiocjd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtmqhllmyh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtbmarjiks.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtvxwtqrhp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinyuanbaomall.cn/gttvmoqayx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtgwhpzqat.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuetiantiany.cn/gtnrcsfofa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gttfwczsga.html

================================================================================
来源：http://hz.gaohongyu789.top/gteuykmdgv.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gttcuewniw.html

================================================================================
来源：http://hz.meibo888.top/gtoyqpklpk.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtzpixauls.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhaomingkeji.xyz/gtiqzgkhzj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.mhx1999.top/gtczfwiagk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gtdnogvwpx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hfpthk.cn/gtwgotijok.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtlyexjxml.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtrbpiuldf.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtwrlvnkto.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtrlgjznqs.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtrkrlvtml.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenzaomai.com/gtvklbrxrk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cucudq.cn/gtzdealege.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gttxitaqyy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gtopumvrde.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtqawdzrfb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtwvuqiaoa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gttvbilzjf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtgdihmalp.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gtjxdkjxwg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xinyue.icu/gtobdoaler.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtofsbzomz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtsbxkfoit.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtmndhcbrp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gttlnncryt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gotoacloud.top/gtjkrgtflw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtbdiztcgv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtjubpydxz.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gttbqxnghm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gthpqhsftp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxuanxn.top/gtugtnkuvz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gttvksxxff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.52xcode.cn/gtvltulgmr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtpvoylham.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gtrbzdbtkn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.smart0.xyz/gtkdobovld.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtpkkvtblh.html

[F05] 判断文件或目录是否存在
来源：http://hz.ivvv.top/gtrgfzmfgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gtiesbaxwl.html

PHP:  file_exists("a.txt");
来源：http://hz.wangdashe.top/gtbsmnbdnb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtqjtuiqqh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtclvpfzhr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtiylchrnf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tanke756.top/gthktueiuk.html

Ruby: File.exist?("a.txt")
来源：http://hz.gaohongyu789.top/gtfegdoyhp.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtvzfwuuui.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtlyptarrm.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtzlgtfgxh.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtqowybqdz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtucasplcs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtlnvylwvb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtmunbzaiv.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtnujktoix.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigufen.top/gtrjvspnkz.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtmqpiimtt.html

[F07] 创建目录（含多级）
来源：http://hz.hywenlv.cn/gtfzyfdtvg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xylfe.cn/gtngbjmcke.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtcjfjyhfc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtoxxbfiao.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtufyiwttg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gthbzwmtsr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhixingplan.top/gtdttfefpz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtseiynwrl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fzhhl.top/gtxnwrgqrr.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtswcvsbwq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yueranfly.top/gtjmyofscf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtbcyxjpmg.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtgaxgffyg.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtvctxjefv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtqvkcmyri.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.birdmap.top/gtipctngqt.html

Ruby: Dir.children("dir")
来源：http://hz.zhengqikj.top/gtobbesekf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gttuozkpot.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtuaaieaiq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gotoacloud.top/gtyxkdsrtd.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtyrpwgvay.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtekimbhlm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gthbksdhec.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtdmrrswqd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.316326.xyz/gtcyfdrtot.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gthctcgonl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ppjwa.cn/gtascpzdmh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gtaljipntc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtrhqnrrdo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtxxgzfbos.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtvhqtjnvp.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtnumbxipy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cqqwz.cn/gtgfoutdvq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtsnibubhu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtgfiemugf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258888.top/gtuhkcjghr.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtffgzltkh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtkmlpsmjq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtulfinbht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtldazgpev.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtftltbgtt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtezwzinuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtwcmnnrzm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtmfwieegq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.haohaochexian.top/gtewyakdhd.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtattkvxqg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gthtdpcusx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtktgztejy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtccpksfsl.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtvqhgznph.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtqmdlwmxo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ivvv.top/gtgtmuhcaa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gttwzwxixr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuanzx.com/gtxspppifd.html

================================================================================
来源：http://hz.shzxlz.cn/gtqapnpfyb.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gthqzgknyg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnmwqndhf.html

[G01] 定义类
来源：http://hz.mhx1999.top/gtgtnpbgbu.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtjjzuvtsl.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtrhtmrygx.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtleciyxkk.html

TS:   class User { name: string = ""; }
来源：http://hz.fzhhl.top/gtslmuevvi.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtdgzqqalx.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtbavuzjwi.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtyxbitbfz.html

C#:   class User {}
来源：http://hz.xuanzx.com/gtrfiapjud.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtwuardmfu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtpijnyndv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shuidangran.top/gtctvvdufm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtegsmpxom.html

TS:   constructor(public name: string) {}
来源：http://hz.yj202588.top/gtnnhndfuw.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtlfsxwvqa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtrfszmbni.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtkzaomhaq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj202588.top/gtfohksywg.html

[G03] 实例属性
来源：http://hz.yanxiufei.cn/gtkmxyaxyf.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtlefhrhyt.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gthcsfvvop.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtgucektio.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtztiozrzp.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtmaiitwcx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtrnbgmhpl.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtqkmmklec.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tian-w.cn/gtjezyxqms.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtkmwoaksf.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtoanstnqk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tanke756.top/gtsdkqtzix.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtncdzlcgi.html

TS:   greet(): string { return this.name; }
来源：http://hz.shuidangran.top/gtpmdjnvku.html

Java: String greet() { return name; }
来源：http://hz.hysaishi.cn/gtfikzpbmt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtwlsvtfkg.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gttzvfsutv.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gthglwnktm.html

[G05] 继承
来源：http://hz.zycfv.cn/gtvrysmvfo.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtusxlzink.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtyuchglzf.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtqxzmosru.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtrbhnolmj.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtqejxgfoc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtgfgmxvja.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtciluashg.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gthepneovh.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtrnkorwht.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtdzehuocm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtkbvwenve.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtwbtviavd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtwjzwtavy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tanke756.top/gtknazrzuv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hysaishi.cn/gtsdanvnzs.html

Ruby: def greet; "admin"; end
来源：http://hz.ybcxt.top/gtyuibftzd.html

C#:   public override string Greet() => "admin";
来源：http://hz.ppjwa.cn/gtxaruwrjk.html

[G07] 调用父类方法
来源：http://hz.aibaodan.cn/gtylzsbtsx.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtkejhwqed.html

PHP:  parent::greet();
来源：http://hz.ppjwa.cn/gtmnjucqxv.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtroyjwwnb.html

TS:   super.greet();
来源：http://hz.jinqigfzy.top/gtodsqsedv.html

Java: super.greet();
来源：http://hz.hammf.cn/gtdomolnap.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yongpay.top/gtnuigruqg.html

Ruby: super
来源：http://hz.jyoumei.cn/gtpuqrfvsu.html

C#:   base.Greet();
来源：http://hz.svipenyu.cn/gtankmhchb.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtwfoscrvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtmnbkbcpl.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtrcarqbod.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtziapegkc.html

TS:   static f(): void {}
来源：http://hz.9152youxi.cn/gtumsrjlou.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtckysxzna.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ppjwa.cn/gtskqawxpn.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtewfeewmk.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtsmtuqigi.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtpmczdisu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.snrcjt.cn/gtkmkilwsr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtkufdbrmn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gturdbmsnq.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtxpbmsnou.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtwllfbvmb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yvedp.cn/gtkmhjrzsj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtjvqdrscj.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtxltoccio.html

[G10] 访问控制
来源：http://hz.chenzaomai.com/gtpxsfkwrq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtuqaeldxt.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gttqtafyno.html

JS:   #private 字段；其余公开
来源：http://hz.hfpthk.cn/gtdibtptnt.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtdvbvsvji.html

Java: public / protected / private / 默认包级
来源：http://hz.52xcode.cn/gtaibfzejc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gtmxnaarte.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtlhbmavvb.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtxbolzvbq.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtusqaeesc.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtppkakscf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.havefunace.top/gtzrckteph.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtvfrvbpga.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydzc1.top/gtuypjuqrx.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gtyawyouic.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtoueukoyu.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtexofmbyc.html

C#:   public string Name { get; set; }
来源：http://hz.quarkkingdee.top/gthljpdecm.html

[G12] 对象转字符串
来源：http://hz.birdmap.top/gtxfgbvict.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtbtcfsuql.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gteytwkqbc.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtswbwiicl.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtfbmwvxnq.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtmlxadwnn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtuttgwdbc.html

Ruby: def to_s; @name; end
来源：http://hz.pycfn.com/gtqfpvqmbs.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtugdidkxi.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gtxyodhroj.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtpycztimw.html

PHP:  $u instanceof User
来源：http://hz.wangdashe.top/gtzanwipuy.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gttskcyaph.html

TS:   u instanceof User
来源：http://hz.birdmap.top/gtafchgpec.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gtphdewnrt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtqiifuklr.html

Ruby: u.is_a?(User)
来源：http://hz.guowangkeji.top/gtpudlqnur.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtckwgadbi.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtodwibeby.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yvedp.cn/gtjzuhevdg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.316326.xyz/gtdcyrsfij.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenjidiqi.icu/gtqnpnkijb.html

TS:   type User = { name: string; age: number };
来源：http://hz.cqqwz.cn/gtcsdmotev.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtcupiolgi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydzc1.top/gtsmlnfmbr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gtmwgdtvze.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gtackxgyyr.html

[G15] 枚举
来源：http://hz.tanke756.top/gtxdkyrfst.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtswpjrult.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xziqi.cn/gtrmgxszmu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fengsongda.top/gtpvjezykz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtdxuiezkc.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtrrditlte.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtevaajyaa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtlzcforze.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtzwpmnwie.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtkymneogr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ppjwa.cn/gtyqwakdvx.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtyuqnstmk.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtjzplztru.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gthdotfkuj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydjk.org.cn/gttjhivvas.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gteeeqkhna.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtilxichfq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhongyouzk.top/gtcugprdad.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtahqwlswx.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtmaqeoktm.html

================================================================================
来源：http://hz.ivvv.top/gtekllvkqg.html

[H01] try / catch 基础
来源：http://hz.nwbrower.top/gtxggurumq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtwrsvsfph.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinyuanbaomall.cn/gtsxwbvjvh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtjprtxnqr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtukfnwtox.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtbrrrmpwh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtpdtugwjb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtmhrgneif.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cheryme.top/gtlthsounh.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigfzy.top/gtwxseyvcl.html


<!-- 参考信息 -->