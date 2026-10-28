代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtoyjtpbrz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.c1oappe.top/gtikqphsxt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuetiantiany.cn/gthapbcpsy.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtaiuwctps.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.havefunace.top/gtjwzsddfv.html

================================================================================
来源：http://hz.sxryk.cn/gtjwpqtyhs.html

F. 文件与目录
来源：http://hz.yj202588.top/gtfccmwmke.html

================================================================================
来源：http://hz.shuidangran.top/gtufbddlth.html

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gtsgksjwsq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtxzqbogut.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtrzfegcri.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtdbzrfjao.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtxuhkdnug.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtglhyozlq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangdashe.top/gtrcqhrfwj.html

Ruby: File.read("a.txt")
来源：http://hz.cdnleiting.top/gtfhzkwxoy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtvrewpmtr.html

[F02] 逐行读取文件
来源：http://hz.cqqwz.cn/gttxrqsdhg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gthhirwekz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtuppkdohx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtwwalymvk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtjyaijtnf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtdkozneok.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gtqtqiasmx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gthjdfzetx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtsvsxwtze.html

[F03] 写入文件（覆盖）
来源：http://hz.meibo888.top/gtiwdyqvhm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jiagoushi.top/gtzdbvmrec.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtiwbbsuel.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtujjtpmlc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtftlzkigr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtnzebwtge.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtlgwgnzth.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangdashe.top/gtsixilsno.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gthvsvtdgv.html

[F04] 追加写入文件
来源：http://hz.aizwys.cn/gtuorxpgqp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cashguo.top/gtltsiqqrd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xylfe.cn/gtaqxyvwcw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtiqwotrpq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtonlbrlqe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtobtbnppx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtmbhtzodt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenlongwang.top/gtooypqtkj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtdcgqwoib.html

[F05] 判断文件或目录是否存在
来源：http://hz.daxiang520.top/gtdulsroqk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtxnokvklp.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gthmkbvvge.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtgtqrmmro.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtpfmiqgyd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtvsftpdey.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtxjkamgbg.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtynvhuoae.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gthsegflem.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtqlxgqfar.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtqiurwiyh.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtlimexbnp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtzcnhnubh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtnkjjnzxr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtyhaszucw.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtdfptxorc.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtjlexjqep.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gtdxmmcccx.html

[F07] 创建目录（含多级）
来源：http://hz.jyoumei.cn/gtpkzfxcqp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtfzpjdgws.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtihwxniuc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtsganouvf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtskgpmpwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtjdtokouf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yueranfly.top/gtegwktnmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gthqnwwkzz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtevhfdjux.html

[F08] 遍历目录
来源：http://hz.snrcjt.cn/gtstoqieif.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtaydnzrcw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sufxvd.cn/gtkpphsvbq.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtrxssurvw.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gttcvdjikw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtprimbbox.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtlhsovufs.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtmxlboeqn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jianghu66.top/gtcfnarmch.html

[F09] 获取文件大小
来源：http://hz.0kj1m.cn/gtmopoymfo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqwvxpxea.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtkulekbaf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gtgtglxbow.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtidvzgszw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtlijddyyo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gtwnmmlssn.html

Ruby: File.size("a.txt")
来源：http://hz.ydjk.org.cn/gtjqpmpvgx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtczyhmsgh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtfiqwhyoa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtsjqkdawx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtzdodzcno.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtmizpisan.html

TS:   path.extname("a.txt")
来源：http://hz.fengsongda.top/gtogetosec.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtcdhpayhx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtxvshvscw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtrtjiddrr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhixingplan.top/gtocpxqyjs.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtgswiqqjn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtygyvdqqe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnxiangtu.top/gtwyoeixeh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtmtstnriq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtqljvczca.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtxmgxprdv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtxchcryju.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtusruyczh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtccnokgng.html

[F12] CSV 读写
来源：http://hz.zhengqikj.top/gtsixruwed.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhongyouzk.top/gtxrfcgdsa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtamqeeval.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtqvzvcryl.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtcjgvgtek.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtqcbtmnkv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtcgihggxq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtcdrdkama.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.0kj1m.cn/gtrlyjxxmb.html

================================================================================
来源：http://hz.nwbrower.top/gtiwyczyhk.html

G. 面向对象
来源：http://hz.yuanzhike.top/gtitsckiqd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvnznrgca.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtflseqgam.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtfgfdgsnw.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gthlfywsrv.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtioymmthg.html

TS:   class User { name: string = ""; }
来源：http://hz.jyoumei.cn/gtzvhzcrag.html

Java: class User {}
来源：http://hz.pengpengdd.cyou/gtpabdkuce.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtcsklxawc.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtnhdlngim.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtqmwujvzg.html

[G02] 构造函数
来源：http://hz.quarkkingdee.top/gtcyrfksxk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aibaodan.cn/gtbwqwfhqp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gttgjzesom.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtgskyqnlq.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gthmhyvtlm.html

Java: User(String name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gttghwxnpg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtdtcltaix.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtcypqlbjq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.redwolf501.top/gtmioscesu.html

[G03] 实例属性
来源：http://hz.ydzc1.top/gtqhwvmjer.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtbvfoxiqz.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtfvmyraua.html

JS:   this.name = "x";
来源：http://hz.zhiwuduotai.top/gtvosgsqqr.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtgkjnqfhs.html

Java: private String name;
来源：http://hz.redwolf501.top/gtwxnkgrda.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigufen.top/gtzdocozie.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtcyiuedor.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtroimdyvf.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gthshvuoaj.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtlojijtme.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtkddjzwqj.html

JS:   greet() { return this.name; }
来源：http://hz.xinyue.icu/gtmzxjtdpz.html

TS:   greet(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtgrmjlfum.html

Java: String greet() { return name; }
来源：http://hz.jinghuilouyu.cn/gtnkrcuiru.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cheryme.top/gtsxqbvryz.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtukuwxeey.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtozeihfqa.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtybznukdd.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gthvktyfna.html

PHP:  class Admin extends User {}
来源：http://hz.ppjwa.cn/gtrkhnrbrs.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtockybeak.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtfknzaqzr.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtjtfehedp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zycfv.cn/gtomeomiam.html

Ruby: class Admin < User; end
来源：http://hz.andypj.xyz/gtruqodsjc.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtboasfpyr.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtqcedggdy.html

Py:   def greet(self): return "admin"
来源：http://hz.shangyingyoupin.top/gtfcciyrjr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtucnzghzx.html

JS:   greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtrgkhzpat.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtxgcdfkaw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtxowmhjlg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtfqvpivrm.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gthhrqldlt.html

C#:   public override string Greet() => "admin";
来源：http://hz.0kj1m.cn/gtrnpxulcj.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtrehcbfch.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtcbhggmkz.html

PHP:  parent::greet();
来源：http://hz.xuetiantiany.cn/gtxpycnfgf.html

JS:   super.greet();
来源：http://hz.cqqwz.cn/gtbeofqiyd.html

TS:   super.greet();
来源：http://hz.andypj.xyz/gtklnwrsso.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtfrufnnrd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gtgwnxjfjy.html

Ruby: super
来源：http://hz.tianlin.xyz/gtcatxlhky.html

C#:   base.Greet();
来源：http://hz.jinqigufen.top/gtiymtsovh.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtfnffogyy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.andypj.xyz/gtqlwngzhm.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtxlxmkzrc.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtvvnmauiw.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtdkknijjr.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtmeywemqj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhoulong.xyz/gtsehhxtqo.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtzjafttoy.html

C#:   public static void F() {}
来源：http://hz.chenjidiqi.icu/gtbdugkzrw.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtjghytoyo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtwinnpdmd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gtmtwmebiz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ppjwa.cn/gtmmalwlcv.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtzvmnvnok.html

Java: interface Shape { double area(); }
来源：http://hz.cdnleiting.top/gtprvryswm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gtpbolfkan.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtsriftial.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gtpfiwmash.html

[G10] 访问控制
来源：http://hz.birdmap.top/gtbjaeborj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ybcxt.top/gtnqstdvax.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gthszohcpx.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtwdacrmwu.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtrmjichcp.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gthkbuimyy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtajnpanzd.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtsvejqpyx.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gtoqaoqbum.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtvvfcmqkh.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtiqxqwhev.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtxesjiset.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtyfxaqcdq.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtxnmbdgaa.html

Java: public String getName() { return name; }
来源：http://hz.iojbl.cn/gtfbdkbekm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtkbofywsr.html

Ruby: attr_accessor :name
来源：http://hz.jinyuanbaomall.cn/gtqkxzbtho.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtirnfzsqf.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtpscbxfmu.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtraultavv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtjhsguixx.html

JS:   toString() { return this.name; }
来源：http://hz.ydzc1.top/gtpfnwgzws.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtwmrdbmbk.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtyjihiuzd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtqyxoqktc.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtpacnakab.html

C#:   public override string ToString() => Name;
来源：http://hz.yvedp.cn/gtesdouduo.html

[G13] 判断对象类型
来源：http://hz.yongpay.top/gtxocnlmdd.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gtcfnusrzk.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtrxxwcglm.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtagaeclva.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtuhebdtxb.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtmbticokf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtzflxvdnt.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtsqcxblej.html

C#:   u is User
来源：http://hz.gotoacloud.top/gtzbpkcoqg.html

[G14] 数据类 / record
来源：http://hz.tanke756.top/gtfajzbcca.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.havefunace.top/gtfmdrxxah.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtrbfwpnqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtezwdvmxp.html

TS:   type User = { name: string; age: number };
来源：http://hz.pengpengdd.cyou/gtlhmibpfo.html

Java: record User(String name, int age) {}
来源：http://hz.havefunace.top/gtxrpnxebm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tianlin.xyz/gtrltdqogr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinghuilouyu.cn/gtkaiajrrw.html

C#:   record User(string Name, int Age);
来源：http://hz.daxiang520.top/gtqvtnaole.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gtijrhsjxd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gthyvynxcf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gthzjljthr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtrnbkwscn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtcppthjxq.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtrqvxvhsv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtasdozkwm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hammf.cn/gtgzjzdigo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtaimskrpd.html

[G16] 对象转数组 / 字典
来源：http://hz.zhiwuduotai.top/gtleopguon.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dashuyun.cn/gtdmvvqsfl.html

PHP:  get_object_vars($obj);
来源：http://hz.sweek.top/gtlmmdrmzu.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtrgqtoxzv.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtxwvnbsfv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtkysxkhgu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtmeqmwxoo.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtwyynnhoj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cqqwz.cn/gtkhtzdsjm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtuwwygfwn.html

H. 异常与错误处理
来源：http://hz.vqdsnc.cn/gtcgpkvzdu.html

================================================================================
来源：http://hz.haohaochexian.top/gtsxfdtvtn.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtaxktlqbg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigfzy.top/gtnrhkzjfe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtehxcasrs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hywenlv.cn/gtlkkjxcxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gtatbedchn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.0kj1m.cn/gtiutovwlb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnqzz.top/gtbfbvoavj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtemsejlxl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gttywzpnky.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtbxzicdag.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgufenzy.top/gtehvcjoty.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtuouycszo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtnrclakvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtyzebhbtp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtsozpqcan.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dianchejie.cn/gtkrlteehe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinyuanbaomall.cn/gthokwalph.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtghhdjxef.html

[H03] 主动抛出异常
来源：http://hz.birdmap.top/gthajilomf.html

Py:   raise ValueError("错误信息")
来源：http://hz.tian-w.cn/gtrobtgpyx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtrhpyytzi.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtdyqkzuny.html

TS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtzhykirzu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gtndsymqzr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtovpphsdh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtzatuprfs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtjwqbalpo.html

[H04] 自定义异常类型
来源：http://hz.birdmap.top/gtsztbnjln.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gthfppfzuo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gtdbzgobpg.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtdfyoimdo.html

TS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtjserhnbq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtrlixpqgl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtgklyyhsz.html


<!-- 参考信息 -->