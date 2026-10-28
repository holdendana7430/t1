代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtpqfogzsz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtnaovvooh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtkiuviqqy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhixingplan.top/gtqlaauzha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.0kj1m.cn/gtsmlhwxxh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtxtjjmpvh.html

[F03] 写入文件（覆盖）
来源：http://hz.xylfe.cn/gtvybqsrec.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigufen.top/gtrtqznysz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gtoqkpmeao.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtuogcknop.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gterqtlpeh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtcnyjvoyq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yangfankeji.com/gtobppuwew.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtabltpolb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gtjvyrvtrs.html

[F04] 追加写入文件
来源：http://hz.52xcode.cn/gtjaypigza.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtvydqohzj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jyoumei.cn/gtmerggwcu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtdbfxkkwt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtafywhneo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ybcxt.top/gtwdkrnlrt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258888.top/gteuokytac.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtwyvatbtd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydjk.org.cn/gtpaklhshg.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtaglrkrsa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtzensldks.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtjzskauny.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtysjdavku.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtgenfwipu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtorgynvlt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258.top/gteglvroww.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gtswbibmwl.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtbjaadnth.html

[F06] 删除文件
来源：http://hz.ehwqpu.com/gtcuiildhw.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtsxgrvkmh.html

PHP:  unlink("a.txt");
来源：http://hz.fengsongda.top/gtbcrgfogt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtmkiouhnn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gttaceesiu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtjbpxniqx.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtyfgjrmrd.html

Ruby: File.delete("a.txt")
来源：http://hz.jyoumei.cn/gtuxnclehz.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258888.top/gtgmyfrhja.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtlmvvdvtn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sxryk.cn/gtxndnfxlb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtdeptwjxi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtcdcbfied.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtwxnchflv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenjidiqi.icu/gtjshzgiec.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtdevntxuj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuanzhike.top/gtqknzamga.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ehwqpu.com/gtydyfahda.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gthfevdwlp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gzhubu.top/gtjbwoanif.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtfppwwgqd.html

JS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtwgrkddwu.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtsfixvsug.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtfmgqldkh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gthszwagyr.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtsleysdhr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gtnsdmbmiu.html

[F09] 获取文件大小
来源：http://hz.xinyue.icu/gtucrqrfsq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtneknxwbk.html

PHP:  filesize("a.txt");
来源：http://hz.fzhhl.top/gtdokfndpd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtaiewfwzx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtwzzbtyko.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gthgnpxxma.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtcunmrioj.html

Ruby: File.size("a.txt")
来源：http://hz.ppjwa.cn/gtrbbqmhtg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.meibo888.top/gtzgrptbyk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.mhx1999.top/gtyhbkstzb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtsqikulor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gtkespfxvp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtqgsyrtzr.html

TS:   path.extname("a.txt")
来源：http://hz.zhiwuduotai.top/gtduolvtov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pycfn.com/gtswoufzfh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuanzhike.top/gtkgnzfbxo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtkkpaedqo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtivpiwnrq.html

[F11] 复制与移动文件
来源：http://hz.smart0.xyz/gtsleamnkl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtxmglxlcy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtymkcwchf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtfrzbdzgr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtwhqptyno.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtpmvzbfrt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtkcagmhvv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtdqvgubxm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtkfhybjkc.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtqpbxahth.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtbgyyuuzx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtmyndacrc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtqbyiongo.html

TS:   // 同上
来源：http://hz.nanxinkj.top/gtyexijvsg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtplvvwpjc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtpodmipzk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gthyplzucg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtutbhklqr.html

================================================================================
来源：http://hz.bjfxy.top/gtlcevaoit.html

G. 面向对象
来源：http://hz.cheryme.top/gtxnixrofi.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkapbhvrc.html

[G01] 定义类
来源：http://hz.cdnleiting.top/gtvxzxxzce.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtaejfzcdp.html

PHP:  class User {}
来源：http://hz.shzxlz.cn/gtdmnwshxr.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtcmeazlto.html

TS:   class User { name: string = ""; }
来源：http://hz.zhoulong.xyz/gtntqjivde.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtpcpqppqa.html

Go:   type User struct { Name string }
来源：http://hz.jinqigfzy.top/gtlqadyxiw.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gttcjskgrk.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtybfmodkp.html

[G02] 构造函数
来源：http://hz.jiagoushi.top/gthooedsqm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtvburdesh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnxiangtu.top/gtlazzlrdn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtyyatymtn.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtrmtkgvmu.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtkszngwyo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtgpmsmpbm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinghuilouyu.cn/gtqdwviepu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtnqpepkxh.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtmmcjgxfz.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtbnmreopk.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtvqstfkxu.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtoopinlfy.html

TS:   name: string = "x";
来源：http://hz.chenzaomai.com/gtvyrejvhg.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gthnimsgeh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gttwlbyjnc.html

Ruby: @name = "x"
来源：http://hz.zhengqikj.top/gtaqhuttcs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtidztnzsj.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtrlqzttuz.html

Py:   def greet(self): return self.name
来源：http://hz.hywenlv.cn/gtheceihmq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gteyldpwsn.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gteylvijlo.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gthwaoxbty.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtitxegvqp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtpwgiyhox.html

Ruby: def greet; @name; end
来源：http://hz.sweek.top/gtypczkixi.html

C#:   public string Greet() => Name;
来源：http://hz.xinyue.icu/gtipbpkbyi.html

[G05] 继承
来源：http://hz.iojbl.cn/gtttnexdse.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gtoryyblrq.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtpapwifmt.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtenefqbxe.html

TS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtqlcxslwi.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtahhsllta.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtsjkcqvau.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtzbycncni.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtxuzokwgl.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtlbezurqp.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gttfdfjcrj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtwibocrfs.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtcfhdbxig.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtdukkpypk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtttuouygo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gtxeycxlar.html

Ruby: def greet; "admin"; end
来源：http://hz.daxiang520.top/gtptscotwv.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtgzsdscew.html

[G07] 调用父类方法
来源：http://hz.hfpthk.cn/gtdnbezsks.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtwvkjefwy.html

PHP:  parent::greet();
来源：http://hz.hongshengwenyu.top/gtdpacvysw.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gthkdzdhko.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtxgqgpjpx.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtawefsthh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtxmuenigw.html

Ruby: super
来源：http://hz.yuxming.cn/gtigmjpsfb.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtjfqydgwt.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtudihcomn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtjykkrhsi.html

PHP:  public static function f() {}
来源：http://hz.tian-w.cn/gtezewrbfp.html

JS:   static f() {}
来源：http://hz.0kj1m.cn/gthkggquzt.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gthcobvuoi.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gtwhibnrhe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtgyysvwwi.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtqqiqxigu.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtcpdtiwnj.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtaudqhulq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gtjympnqun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gteyjdhkgx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtnmzytzzy.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtzmzwqptk.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtjvbsgvvc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj202588.top/gtngqoqwug.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtfzfcpvdp.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtjdghuzmz.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtqdzjajlm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtrtiilihz.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gttrwershz.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtkbomxvko.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtbupuinoo.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtmueinckl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtijfxjovl.html

Ruby: public / protected / private
来源：http://hz.316326.xyz/gthqtisipe.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtlrjtbczw.html

[G11] getter / setter
来源：http://hz.hongshengwenyu.top/gtklcyewsp.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtdqipgrrv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtqvztcavs.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtuhgkbkaq.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gthropidit.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtvsssnadl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtqvekoodm.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtsydnojjj.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtuzobfibs.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtwcikvthr.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtelogdvcv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtcubndaqb.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtqiwzalnm.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtyndnfchj.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtohimlskm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zycfv.cn/gteurttnhy.html

Ruby: def to_s; @name; end
来源：http://hz.nanxinkj.top/gtiuuyuvrk.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtelycisds.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtavtxonck.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gthbttmfdr.html

PHP:  $u instanceof User
来源：http://hz.wangdashe.top/gtnqvoqubd.html

JS:   u instanceof User
来源：http://hz.ydzc1.top/gtzwjduwwr.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtmqjrgsri.html

Java: u instanceof User
来源：http://hz.316326.xyz/gtugucwnve.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtivediasp.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtfajuelde.html

C#:   u is User
来源：http://hz.hongshengwenyu.top/gtxtrbmgre.html

[G14] 数据类 / record
来源：http://hz.smart0.xyz/gtyvjqauji.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shzxlz.cn/gtmzzqyjrl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtnxalvsxd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtvhbzqxlq.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangkeji.top/gteeywmfou.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtsierfnwz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtcixcmlcm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtuymmgpxs.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gtvoiptqzd.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtfznhjyce.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.smart0.xyz/gtbbsphhbb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnxiangtu.top/gtbvjtegnq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtokipaxxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtqqoxfwml.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtnwndjbpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gtcloqrxih.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtovyssiea.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtjgcemkxx.html

[G16] 对象转数组 / 字典
来源：http://hz.xylfe.cn/gtojwohjlg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daxiang520.top/gteaohcndh.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gtlrvqrvqw.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtodblfvgd.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtmmwfnsrp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gtawmtjxke.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtwlwivgnd.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtvtdonjua.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.meibo888.top/gtsmbdsrlo.html

================================================================================
来源：http://hz.pycfn.com/gtqnljknpc.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtnxtohnxy.html

================================================================================
来源：http://hz.yj20258888.top/gtzwwukpmt.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtghjffkxd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtwdhyazxh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtxxgbchkd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtmonjedfx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtnqmrzrjk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtapcjzjan.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sxryk.cn/gtsytvbdex.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtnhoxycvu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgufenzy.top/gtzvaswncg.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gtkkmardcs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.bjfxy.top/gtrqwmtcux.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtmftallfp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtzwvhmmkk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtcgtpguqq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtkpyzmtlv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtbuturdnf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daxiang520.top/gtidqsagoy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gttuvodhwg.html

[H03] 主动抛出异常
来源：http://hz.ppjwa.cn/gtdlufsmdx.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtylemdwfu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtachsgsts.html

JS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtimblroyv.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtbiqdfdfv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtlkojobay.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtaqtuyupy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtqlmgemfa.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtwqobftdn.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gtqnurxkep.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtfuhjwuon.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtxxhjvaei.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtzgsmxmgq.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtdeanlfro.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtfmahzvph.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtnkxgujtv.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gtfmiupgyr.html

C#:   class MyException : Exception {}
来源：http://hz.andypj.xyz/gtfwbpjcvk.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtryerqvcy.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtclreykqv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shzxlz.cn/gtvsthzmwy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtsqfsryct.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtlhfyritv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ivvv.top/gtwvcermhe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtqlfevztn.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtzcidihec.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tianlin.xyz/gtwegkczdw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtpefmvmba.html

Py:   value = d.get("k") or default
来源：http://hz.wangshuangyany.cn/gtenytjore.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtbafahwwb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtemdevomg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtzkhupamc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtudvvmdpm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gttzfrjdga.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangtech.top/gtzbmdooqf.html

C#:   obj?.A?.B ?? default
来源：http://hz.xylfe.cn/gtgqwfysew.html


<!-- 参考信息 -->