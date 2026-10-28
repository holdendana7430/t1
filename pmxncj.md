代发 wailian999

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtilpaywnq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.havefunace.top/gttmhzwmml.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnqzz.top/gtwlaztjud.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtlfsnciat.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fengsongda.top/gtecdvnvaj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gteayrgasq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtzymlmtnz.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtlbffadbc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtjioguyqi.html

[F02] 逐行读取文件
来源：http://hz.yanxiufei.cn/gtcwbziims.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtouggoxdk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtszhbsrfe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtxfwbraco.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gtstbpjicg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtlzhxegbu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhoulong.xyz/gtqewrwisj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtnimrlzvd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.quarkkingdee.top/gtfmhhkxzk.html

[F03] 写入文件（覆盖）
来源：http://hz.zycfv.cn/gtpgmelibn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuanzx.com/gtxnpnists.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guannengcc.top/gtxktaqktn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtinxcypfq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtnaydowxm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ehwqpu.com/gtfscbkaxy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gtuatqddey.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gthenfwtdn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtiyuvsnkg.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtiiurmnwh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hfpthk.cn/gthayecbfw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydjk.org.cn/gtmsjcbvfe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtsvaukipl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtsoppejhy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.0kj1m.cn/gttxnfqxlc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtwlicshkz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtvxhkauip.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cheryme.top/gtpekgzljs.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtgyyfkxou.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aibaodan.cn/gtwddcgasm.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gtqfukepzc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtzahakmig.html

TS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtuoptpuxc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtkcqyeoav.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtudpqsccg.html

Ruby: File.exist?("a.txt")
来源：http://hz.cqqwz.cn/gtduedalym.html

C#:   File.Exists("a.txt")
来源：http://hz.zhixingplan.top/gtrcibvmsv.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtzjkagthj.html

Py:   os.remove("a.txt")
来源：http://hz.redwolf501.top/gtxfeyuibr.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtzihlomti.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtdgmdisjh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtqyunhutb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtidjrwvqe.html

Go:   os.Remove("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtzfapgehz.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gttakyhwek.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtyazhwxco.html

[F07] 创建目录（含多级）
来源：http://hz.pengpengdd.cyou/gtycozemtj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.iojbl.cn/gtogfdbdiu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aizwys.cn/gttxsonnnq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtbfwvhtmn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gthrsegysl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtwtxbzyto.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangkeji.top/gttcnqnmwn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtgukhaqcf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yvedp.cn/gtfkidwnem.html

[F08] 遍历目录
来源：http://hz.jlsjyb.cn/gtwmsysubf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.snrcjt.cn/gtjxamtful.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtysansfir.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtmdiywoie.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtqwbksjwn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtcngkhrro.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtktzmrmqy.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtdqnleibq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gttpspjhac.html

[F09] 获取文件大小
来源：http://hz.cqqwz.cn/gtfitcvylv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gtdrnrhkae.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gtrmfsnwqp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtfjlwslgo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtcaainlne.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtgaukoisv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtrfokxzse.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtfuwvgqgl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gtyvgznfbk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtsmbijefe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtffbmsthu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtzjknpnmy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtdjxbbqil.html

TS:   path.extname("a.txt")
来源：http://hz.tanke756.top/gtrfzpknrh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtbjiyvgzx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtwpmwmqfr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtxkxedbrm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gthorobhhe.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtjvigagte.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtggxooupn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.52xcode.cn/gtkxvucyiq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtksdurrpp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtmqmtvxtv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gtwooelash.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtyrjaapcl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtnngwjpqg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.bjfxy.top/gtimrghdse.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtndkucsfe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtfctpemlp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xziqi.cn/gtyzugluzy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtpppabwaq.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtkdmtzkvu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gtrnhvygdd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gturuqzpvn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtgqacupsm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtvidnvdrd.html

================================================================================
来源：http://hz.zdqjudy.top/gtgrnanzhh.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtcwqzompl.html

================================================================================
来源：http://hz.yj20258888.top/gtanilswdo.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtbrqpgusr.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtyeuynjoz.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gtvitjcvof.html

JS:   class User {}
来源：http://hz.ivvv.top/gtrfyzebut.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtrodwhqwq.html

Java: class User {}
来源：http://hz.ydjk.org.cn/gtzgdokngn.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtutqvjacc.html

Ruby: class User; end
来源：http://hz.nwbrower.top/gtrcwelryx.html

C#:   class User {}
来源：http://hz.ivvv.top/gtsgkpnerc.html

[G02] 构造函数
来源：http://hz.dashuyun.cn/gtzglzronl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sysykeji.top/gtopojrznr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtrcnoomzd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtwotxkfgg.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangtech.top/gtninexbpt.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtoatrgyst.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtsvckqici.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtzvqvqrpt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxinkj.top/gtmqlolutg.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtsmvlusxg.html

Py:   self.name = "x"
来源：http://hz.yongpay.top/gtcqjihbmy.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtknlsuyqn.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtlwykkzkb.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gtoolwpfcx.html

Java: private String name;
来源：http://hz.yj20258.top/gtkpeermtb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenzaomai.com/gtmmahnrxh.html

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtoclsvpbr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gttuzeiobf.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtoldgevmc.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtzsfxgkqu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtvbbyqqlb.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtuxpizysq.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtuvdfsmpu.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtbgusjgkc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tianlin.xyz/gtklneuqos.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtawyehjak.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtnqitadqr.html

[G05] 继承
来源：http://hz.yueranfly.top/gtqeooghgx.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtecrynrzk.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gtnwhwuqqw.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtopynjsag.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtkqbvrljl.html

Java: class Admin extends User {}
来源：http://hz.sxryk.cn/gtsiyoyqeh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtgbjdvcep.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtviumwbjw.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gtmdhapuap.html

[G06] 重写方法
来源：http://hz.ydzc1.top/gtahjmfffr.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtolitsguk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtlimvrtfk.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtgonlkfnf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gteoazaiuj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtrbbavqml.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gttxxcgrhh.html

Ruby: def greet; "admin"; end
来源：http://hz.gogol.net.cn/gtfpcyltyz.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenzaomai.com/gtzlkamdps.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtjviebboz.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtjdzqixtk.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtuhftorsm.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtuosoisla.html

TS:   super.greet();
来源：http://hz.316326.xyz/gthpjexbeb.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gtvnhjescb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cheryme.top/gtifnpmdqe.html

Ruby: super
来源：http://hz.jqgfzy.top/gtbvapvlby.html

C#:   base.Greet();
来源：http://hz.gzhubu.top/gtnwechssf.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtazzjddsl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gthikgszvk.html

PHP:  public static function f() {}
来源：http://hz.c1oappe.top/gtrymxozqi.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtbbdycfwb.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtufbafxjx.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtzuylsbzn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.9152youxi.cn/gtsbnpahlj.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtxdincunw.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtgsznrjty.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtrevbiqmy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.redwolf501.top/gtxulliczb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gthnfoindk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtxpxnngpe.html

TS:   interface Shape { area(): number; }
来源：http://hz.jiagoushi.top/gtjytrpfon.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtevvxxhgw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtmcvirakf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtbovjhjty.html

C#:   interface IShape { double Area(); }
来源：http://hz.haohaochexian.top/gtpfptxhin.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtabccphxq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtpblrdgxq.html

PHP:  public / protected / private
来源：http://hz.cashguo.top/gtuafojvkh.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtieqrrpsn.html

TS:   public / protected / private
来源：http://hz.tanke756.top/gtjbmyxvzg.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtrbimurdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtirirqrrs.html

Ruby: public / protected / private
来源：http://hz.jinghuilouyu.cn/gtfgttpzvy.html

C#:   public / protected / private / internal
来源：http://hz.hongshengwenyu.top/gttprqpwik.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtiaqvoovr.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtwcdbxghj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gttttjjzox.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtzpzfybkr.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtszxbvalv.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtxbiapvbr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtswxbqoro.html

Ruby: attr_accessor :name
来源：http://hz.andypj.xyz/gtpzaxmbdg.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtbfizuftp.html

[G12] 对象转字符串
来源：http://hz.dianchejie.cn/gtcihuwfjs.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtvsxlpynm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtvecbqkou.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtyjyoxyal.html

TS:   toString(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gthlqouecb.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtbxpbqdlo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtrqfikkgj.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gtyfnrrmxw.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtapyrdsxi.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtyhfvzzne.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtpjuctpxw.html

PHP:  $u instanceof User
来源：http://hz.xylfe.cn/gtwjqmnyhf.html

JS:   u instanceof User
来源：http://hz.nwbrower.top/gtxbohetod.html

TS:   u instanceof User
来源：http://hz.yvedp.cn/gtowrhfrqk.html

Java: u instanceof User
来源：http://hz.jyoumei.cn/gtizbbkbsk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.birdmap.top/gttzpkwejs.html

Ruby: u.is_a?(User)
来源：http://hz.yuxming.cn/gtjehfctcc.html

C#:   u is User
来源：http://hz.feifeiyinyue.top/gtltncafyh.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtzdlnixpj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtzejqzexa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ehwqpu.com/gtpedltfbf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.birdmap.top/gtisvjpmry.html

TS:   type User = { name: string; age: number };
来源：http://hz.316326.xyz/gtvfmvociy.html

Java: record User(String name, int age) {}
来源：http://hz.yonumen.top/gtvlrhumdt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtcxqmmozs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtslihlvvh.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtjhiyibbc.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtxejmwkaq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tian-w.cn/gtukiwmzag.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtkzxvxlpz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtzshxazcn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtqtzbrrek.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtssangpha.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.andypj.xyz/gtzvewlkdk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtmncgunil.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtbtefmoeq.html

[G16] 对象转数组 / 字典
来源：http://hz.daria6918.cn/gtaxdqxisj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cqqwz.cn/gtwvacyvpv.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtivibgntp.html

JS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtktktvwjn.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtshurcmeu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigufen.top/gtgsiktepn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gttbgggvzl.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gtyfkroyia.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigufen.top/gtaebgehxw.html

================================================================================
来源：http://hz.jyoumei.cn/gthaqvoiib.html

H. 异常与错误处理
来源：http://hz.zdqjudy.top/gtxclzvgkd.html

================================================================================
来源：http://hz.jianghu66.top/gtjcqvwnkb.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtzplarwwc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtfseaxctr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gtfonfhvxv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtufqziinr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtcfqeznnu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtkhdfviph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtgvnfwmbh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtokxxzoqy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gteaejzwuz.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtlzlbnzlt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtnojemvho.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtsorfrnha.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtsetgtyxs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtubanrzwy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtivxcoqlc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cqqwz.cn/gtcpbzeqvg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtxqfydnaq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtyyakcqyy.html

[H03] 主动抛出异常
来源：http://hz.vqdsnc.cn/gtkedcinvl.html

Py:   raise ValueError("错误信息")
来源：http://hz.fzhhl.top/gtvwgrahex.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtedmebxqq.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtksbjxtuz.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtkzxxvqhr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gthzmqccbd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtmumkfrwf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydjk.org.cn/gtymjudrpe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtnscogmmg.html

[H04] 自定义异常类型
来源：http://hz.fengsongda.top/gthnzzagql.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtuvnkbecm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtgeeljvbm.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtfjrrbwyp.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtcixvdres.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtvgzrvfoq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gttuusdkeu.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtuyqwbwtf.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtmacdrubq.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtzrhqskzk.html

Py:   except ValueError as e:
来源：http://hz.9152youxi.cn/gtmmjvktte.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.feifeiyinyue.top/gtrrawkmns.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtprqutuug.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gtcwyvyqly.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtkdzehgmf.html


<!-- 参考信息 -->