代发 wailian999

[F01] 读取整个文件
来源：http://hz.daxiang520.top/gtngfgnflb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daria6918.cn/gtuzvcmomd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtcthnxxvi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.316326.xyz/gtstxcnqrc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gtlddhntbd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtlwzqwaya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hysaishi.cn/gthzvwmzlp.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtswsztuqb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydjk.org.cn/gtagkbrjif.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gtnjsxmuvw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aibaodan.cn/gtdewrgtdv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gttwriwqad.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtovzijsyv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtjfnraunn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtxfrbaipv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sysykeji.top/gtpafarblr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtqwamgwnb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gtgbensyqp.html

[F03] 写入文件（覆盖）
来源：http://hz.shuidangran.top/gtxwgimyew.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tanke756.top/gtswtwjhcv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtfhobitje.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtgjovemaz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtydhgracf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtfbldxxdn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258.top/gthctexeol.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtetffhavb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dianchejie.cn/gttmejcjya.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gttdyvlmvz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtnqysifhk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangdashe.top/gtpkragqna.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtaothncag.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtqqkmqkfq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.haohaochexian.top/gtnnszrbdy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtgcxrdyjy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yanxiufei.cn/gtqaouyrsa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gthmcnopyv.html

[F05] 判断文件或目录是否存在
来源：http://hz.ivvv.top/gtowxkppcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtwhhitltr.html

PHP:  file_exists("a.txt");
来源：http://hz.ydjk.org.cn/gtsrqbsvdp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtqmnemdzn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtoyyojtik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtmgamlnca.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinyuanbaomall.cn/gtwhnsmdbx.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gtwomsrofx.html

C#:   File.Exists("a.txt")
来源：http://hz.cheryme.top/gtbayvqfxy.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtdslpodnc.html

Py:   os.remove("a.txt")
来源：http://hz.hnxiangtu.top/gtnutvpzlj.html

PHP:  unlink("a.txt");
来源：http://hz.zhongyouzk.top/gtfmtwdgmi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtnzieieau.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtdyfwenbn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtssqenlff.html

Go:   os.Remove("a.txt")
来源：http://hz.jianghu66.top/gtwyrdgehx.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtxamlvjlx.html

C#:   File.Delete("a.txt");
来源：http://hz.chenlongwang.top/gtvmywjnhj.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtcdfxugfv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtrxirrexe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tianlin.xyz/gtlmiekrgo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtbvagumrw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtylzdxbga.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtknzdmdha.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.quarkkingdee.top/gtqzliadmn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gttjvdeytt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gttehzaknj.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtvnczsxqp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtpuvupaoz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtketamsrz.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtwmdnwenu.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtjzeemvqq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtgyfqghyo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yonumen.top/gttgrsxpox.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtxmhvzjdq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fzhhl.top/gtznfkbsri.html

[F09] 获取文件大小
来源：http://hz.wangshuangyany.cn/gtyizejtpk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigufen.top/gtazvdzwhs.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gthqujynjx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtzxfdpkpp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtztlkiajw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtdlmqhcrl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ybcxt.top/gtfznmyler.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtpmdplxiw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtdwvwwsgr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtekssnigg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtzkvanchi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgufenzy.top/gtbuoyxdlp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtbqnvwtpf.html

TS:   path.extname("a.txt")
来源：http://hz.zhijiandao.cn/gtuqcbtios.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gogol.net.cn/gtnljgfsmt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnqzz.top/gthinzvdae.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtvlpizdtj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guowangkeji.top/gtklrbjtjp.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtvaxwmtci.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtxoiidyid.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtroqgbemh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtqwehazij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtgfhlshwh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258888.top/gtwjaqezgt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtwokgqtab.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtgrsgqxwf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hongshengwenyu.top/gtsxddjgyt.html

[F12] CSV 读写
来源：http://hz.yueranfly.top/gthumagpyj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gtostaltjt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daria6918.cn/gtyoefsasc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daxiang520.top/gtviyhkkbu.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtjtpgsiry.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuanzhike.top/gtjfgbxqxr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gtmputxkbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tian-w.cn/gtdwfwyimv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtyzyhzfhr.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwelsvznh.html

G. 面向对象
来源：http://hz.vqdsnc.cn/gtkrvngsss.html

================================================================================
来源：http://hz.ydzc1.top/gtjnssjiwk.html

[G01] 定义类
来源：http://hz.cucudq.cn/gtqpuzveer.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtsnatpvvm.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtwzovbmuj.html

JS:   class User {}
来源：http://hz.tian-w.cn/gtipapvknl.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtxjfsarqm.html

Java: class User {}
来源：http://hz.nanxuanxn.top/gtgavjqcnl.html

Go:   type User struct { Name string }
来源：http://hz.xuetiantiany.cn/gtrhwyiqqk.html

Ruby: class User; end
来源：http://hz.zhoulong.xyz/gtomhayvar.html

C#:   class User {}
来源：http://hz.yanxiufei.cn/gtmmppkhlk.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtyceeyvjn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gtarcydkhf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtcpwhmzax.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtxabfyuyk.html

TS:   constructor(public name: string) {}
来源：http://hz.ybcxt.top/gtndbwwahw.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtrtpmholw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxuanxn.top/gtguamrcmh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gtuyzfrwae.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gaohongyu789.top/gthuwwbbsm.html

[G03] 实例属性
来源：http://hz.meibo888.top/gteesibjsv.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtusjxcvnp.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gtqgposdyq.html

JS:   this.name = "x";
来源：http://hz.aizwys.cn/gtpbfqklff.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtpooqlquc.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtuyakhfvo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtzhvdnbux.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gthbdtgmsw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daxiang520.top/gtzhqvamzv.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gtqfcdkoul.html

Py:   def greet(self): return self.name
来源：http://hz.ydzc1.top/gtvptyvyca.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtbycpjjgq.html

JS:   greet() { return this.name; }
来源：http://hz.havefunace.top/gtbkngpalg.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtuudmdqlz.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtvfzzirgt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtqzdwqigh.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtsonlkcdt.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtmzzpuypa.html

[G05] 继承
来源：http://hz.zhaomingkeji.xyz/gtusroivxn.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtxtnpdzhd.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigufen.top/gtnykkonyb.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtggqwatdm.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtvfysaizp.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtmiawdgfk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gttibbsysc.html

Ruby: class Admin < User; end
来源：http://hz.pycfn.com/gtpvfydrwv.html

C#:   class Admin : User {}
来源：http://hz.yuanzhike.top/gtauafizjw.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtocypuhqe.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gtekcstswb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtonadyjmk.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtzjguuovk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtypfxeumd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtdfdpuczy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtjbapasfo.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangtech.top/gteywjgqxn.html

C#:   public override string Greet() => "admin";
来源：http://hz.cashguo.top/gtelapqryu.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gthgbqlhlo.html

Py:   super().greet()
来源：http://hz.jinqigufen.top/gtpfutqmhz.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gtuxgkfqmi.html

JS:   super.greet();
来源：http://hz.yueranfly.top/gtkudelwyf.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtsbsjwieb.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtolmrkdip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtllqxkpdz.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtiuduwgao.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtsmquyzbq.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtaygterhh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtrpnrrxen.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gthhoggwbp.html

JS:   static f() {}
来源：http://hz.c1oappe.top/gtsaledbbz.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gthelqfrjr.html

Java: static void f() {}
来源：http://hz.xylfe.cn/gtdtpaiucw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.svipenyu.cn/gtaqjhpzqe.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtnfosphmx.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtxliprikn.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gttwsxalmf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtnpyiawhn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtenzqalke.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtrtpieblc.html

TS:   interface Shape { area(): number; }
来源：http://hz.0kj1m.cn/gtzcbextqk.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtutyonoqp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtggczvsvo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtprhsoffs.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtbzjovrpd.html

[G10] 访问控制
来源：http://hz.ydzc1.top/gtizsgjdes.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtypldnxem.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gthradhlaq.html

JS:   #private 字段；其余公开
来源：http://hz.gogol.net.cn/gtjfcmeodg.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtkvdqcujy.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtexkhtgdb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtgtzvdclm.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtqvnkkmtx.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtiycjcjoh.html

[G11] getter / setter
来源：http://hz.guowangkeji.top/gtnibxvzgf.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gtebkpdqvy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtnpgeioln.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtjrxyitne.html

TS:   get name(): string { return this._name; }
来源：http://hz.0kj1m.cn/gtqvrnqsku.html

Java: public String getName() { return name; }
来源：http://hz.nwbrower.top/gtstnyvcej.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtsvfwitxd.html

Ruby: attr_accessor :name
来源：http://hz.dianchejie.cn/gtrqrnatgv.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gtruqkecut.html

[G12] 对象转字符串
来源：http://hz.cashguo.top/gtcdsodppo.html

Py:   def __str__(self): return self.name
来源：http://hz.zhijiandao.cn/gtgdvlyqsm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtvornvien.html

JS:   toString() { return this.name; }
来源：http://hz.sweek.top/gteicqnudl.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtipgrjtap.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtjkbxhnpj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtvmkuuvyl.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtirkaosdb.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtrorgpgbz.html

[G13] 判断对象类型
来源：http://hz.ydjk.org.cn/gtskpklvfh.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtedddtwtd.html

PHP:  $u instanceof User
来源：http://hz.zhiwuduotai.top/gteavqmosb.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtvqtooibj.html

TS:   u instanceof User
来源：http://hz.hnqzz.top/gtpzhbfxsj.html

Java: u instanceof User
来源：http://hz.c1oappe.top/gtwumyktpb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtawvqdqrv.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtmoswusat.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtbexlmark.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtwzutwymk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xingfuxueyuan.xyz/gtxtyxxhlb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gtujqucjlh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zdqjudy.top/gtujhkdztr.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinyuanbaomall.cn/gtxoyywksj.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gttwcblmpv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtkmzvfzuk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sysykeji.top/gtixmcnesv.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtsptahzdf.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtzfdgpzog.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtopfnsqnm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtoweyxohy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhixingplan.top/gtdsojmyjn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtdnvsyqou.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtuerzvpey.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxuanxn.top/gtuiefqqhf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtwbvuonff.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtlyfmvpve.html

[G16] 对象转数组 / 字典
来源：http://hz.316326.xyz/gtnqqzkmrm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zdqjudy.top/gtgcbfrkmb.html

PHP:  get_object_vars($obj);
来源：http://hz.iojbl.cn/gteldrjnca.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtrzuthxnq.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtrxbecurp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtmnrdzthg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gtoqoaxcfa.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gttqfbhfqm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tanke756.top/gtawepueuz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpvivzdtw.html

H. 异常与错误处理
来源：http://hz.ybcxt.top/gtohdumcpv.html

================================================================================
来源：http://hz.bjfxy.top/gtajibdcnl.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gtwerxbcdm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtzjtjzkgd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtzabeeyyi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtauelsxfu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gteqcsbeio.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtpijrafmu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtkerhmutx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhoulong.xyz/gtrevbewxj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pengpengdd.cyou/gtuaiypvui.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtjvalomtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gteeutebrd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gthqtgsuho.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtwinrffah.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gttahgplsf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtaktiqrzg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtknuznxxq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ivvv.top/gtkfdkrluk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gtsqmyahvq.html

[H03] 主动抛出异常
来源：http://hz.andypj.xyz/gtvupetnrx.html

Py:   raise ValueError("错误信息")
来源：http://hz.xingfuxueyuan.xyz/gtebhgjqud.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtpbegrpwu.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtnjuvlfzx.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtjocnmyps.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gthailkcmu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtedziplyi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gtugyczjyo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtanuctrxo.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtqredkmkr.html

Py:   class MyError(Exception): pass
来源：http://hz.cdnleiting.top/gtculwhnvy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtqgddsbcq.html

JS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtjqjxucnu.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtowsmtmsf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtifkilrxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtdrzlxcvh.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtbbgfhokd.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtagfuokac.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gtoqmlmytv.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtgujrumwp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtlsmoqpth.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtwewdryuk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtuqqkwlwh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtzjgdjljj.html


<!-- 参考信息 -->