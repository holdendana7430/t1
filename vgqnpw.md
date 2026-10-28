代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtnzzyzgvg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtlpsnvtja.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtjakokyej.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daria6918.cn/gtnszwrckn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhiwuduotai.top/gtrlpueeqd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.svipenyu.cn/gtlqzihgzu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtskiwiixx.html

[F04] 追加写入文件
来源：http://hz.ybcxt.top/gtltkcfoiz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xinyue.icu/gtlyvlsama.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.52xcode.cn/gtjzlhkuqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gteoxgwtvp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gthbhwjydq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtkmljhsph.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtjrkzmtxy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jlsjyb.cn/gtkhvspvoe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jlsjyb.cn/gtappvtpaq.html

[F05] 判断文件或目录是否存在
来源：http://hz.gogol.net.cn/gtcuzvocrm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hfpthk.cn/gtlkcqlejj.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtrwnswjep.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtpelbpuer.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtguopcrun.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtrannrxyx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yanxiufei.cn/gtuiahzguf.html

Ruby: File.exist?("a.txt")
来源：http://hz.yongpay.top/gteajzzdhu.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtxhmhibbs.html

[F06] 删除文件
来源：http://hz.ppjwa.cn/gttjoopddm.html

Py:   os.remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtdkovtiwk.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gtfhnuxalx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdtnqbzkn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtvltqsymq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtiqbkodvb.html

Go:   os.Remove("a.txt")
来源：http://hz.cqqwz.cn/gtygbgniqn.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtagriuwfx.html

C#:   File.Delete("a.txt");
来源：http://hz.jlsjyb.cn/gterwbuplv.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtjexxbdjg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgfzy.top/gtlldvqpnr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtxiwwslfz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtbwyyoaks.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtckjoigzs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtoxuqstfo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gtncrydyqd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtznwabxng.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtvoeefuqd.html

[F08] 遍历目录
来源：http://hz.ydjk.org.cn/gtwewnowps.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtdlkqtfzb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gtiigckqvg.html

JS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtjroihvez.html

TS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtaprqgknr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtfwfbbmzr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fzhhl.top/gtxoioxchy.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtnbyfhsdw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtocfeakpw.html

[F09] 获取文件大小
来源：http://hz.yj20258888.top/gtgaifnxqq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gtfdzkpocm.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtbskokbsi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtsycjjtqx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtyjkzejvl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtswgyndte.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gtnwipjaae.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtowyxgheb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gtjtcotedq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtfvzqdquj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtclwabxxb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tanke756.top/gteheiwujb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtxenymrpr.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtghcwxrqj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtnedjqypx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dashuyun.cn/gticnsqdsl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtbtzvzhrh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtwwelpsfn.html

[F11] 复制与移动文件
来源：http://hz.hysaishi.cn/gtfmfrrehs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtkjxumdlb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtdwhrfslz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtrmezgjgs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gthkzmmvzr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gtpmuwuuqz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.quarkkingdee.top/gttmhwpnyb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtyiewuijj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258.top/gtbllinzoz.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gtdpvkyjbp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinyuanbaomall.cn/gtbwvgltmv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtuovucaom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydjk.org.cn/gtxdxssvhp.html

TS:   // 同上
来源：http://hz.jiagoushi.top/gtsncltvio.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gtqxzdbvmc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hammf.cn/gttnekqfqk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenlongwang.top/gtuxfrzazd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gthhifgohi.html

================================================================================
来源：http://hz.shuidangran.top/gtctmaglku.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtyoxjdgjq.html

================================================================================
来源：http://hz.sufxvd.cn/gtzdcqguqu.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtjbavyrnp.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtsjbsmdzy.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtxcdicpzs.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gtjtyvitqd.html

TS:   class User { name: string = ""; }
来源：http://hz.redwolf501.top/gtqddfvqwl.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtsuuwecxc.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gtqthltuyb.html

Ruby: class User; end
来源：http://hz.shuidangran.top/gtvawrwmfj.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gteykyrzqe.html

[G02] 构造函数
来源：http://hz.hnxiangtu.top/gtypmwnqpj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gtznejudzl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dianchejie.cn/gtpwnytpwk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtraslmoye.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtysqvsawa.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtstvfunsx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gtkakezzqy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tanke756.top/gtursqfgvg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtdnzrtycr.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gttqmjgrnv.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtbdauygpz.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtgqgrsuit.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtaqonphmo.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtjjsqxfju.html

Java: private String name;
来源：http://hz.xuanzx.com/gtaicbguel.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnqzz.top/gtvsguyxga.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtcshfotuq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtpktqpgfb.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gttdjkpehp.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtjrykvaow.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtzqbuoggw.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtctgdvmru.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtdgazvakb.html

Java: String greet() { return name; }
来源：http://hz.aizwys.cn/gttnbppooe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtgatzeasg.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtioxbwdjj.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtsujiusco.html

[G05] 继承
来源：http://hz.aizwys.cn/gtdhqhpczl.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtfpkkinsl.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gthmvmjyas.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtxztjqwaa.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtoumhybdi.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtdnmrijoh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtmmdknxsk.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtroyzvnqa.html

C#:   class Admin : User {}
来源：http://hz.dianchejie.cn/gtoziczgwv.html

[G06] 重写方法
来源：http://hz.xinyue.icu/gtmiywxcam.html

Py:   def greet(self): return "admin"
来源：http://hz.nwbrower.top/gtemjzrrph.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtqyosjsvv.html

JS:   greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gttdzlvztq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtgtsdczih.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtekmjhulh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtyobwxuwq.html

Ruby: def greet; "admin"; end
来源：http://hz.zhaomingkeji.xyz/gtpksawprb.html

C#:   public override string Greet() => "admin";
来源：http://hz.snrcjt.cn/gtrtiknmfr.html

[G07] 调用父类方法
来源：http://hz.jinyuanbaomall.cn/gtidpzyldd.html

Py:   super().greet()
来源：http://hz.havefunace.top/gtqowllinr.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gttjqoncbs.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtbwthxovs.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtahkejhgh.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gthvzyadax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.9152youxi.cn/gtpqobufjh.html

Ruby: super
来源：http://hz.yongpay.top/gtajwryuyf.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtekxjwiio.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtswtwcmxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zdqjudy.top/gtjiwubssl.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtzquyxbon.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gthzqcuvrz.html

TS:   static f(): void {}
来源：http://hz.mhx1999.top/gtdqxleauf.html

Java: static void f() {}
来源：http://hz.gaohongyu789.top/gtqlpabjqy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hongshengwenyu.top/gtpmxakdgk.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtswvkhhzg.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtewaedbxm.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtkjmigijv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cheryme.top/gtezaqeolz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yanxiufei.cn/gtppfjwewu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sxryk.cn/gttamhkwew.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtqnwmjlvz.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gttsctucwf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnxiangtu.top/gtiwvsesih.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cqqwz.cn/gtqlocuewb.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtovjtyuft.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtzeyfcytx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtoqdpkvnl.html

PHP:  public / protected / private
来源：http://hz.sweek.top/gtqvneaurh.html

JS:   #private 字段；其余公开
来源：http://hz.sxryk.cn/gtumcbrvdi.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gtddehpvhk.html

Java: public / protected / private / 默认包级
来源：http://hz.cqqwz.cn/gtuolxtwij.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtpirrjoqq.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtvjemxlwu.html

C#:   public / protected / private / internal
来源：http://hz.ywan-chungtsiang.top/gtalgyxche.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtetnhkvys.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtlucdxbwv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtrowzjmmd.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtedqxawdm.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtsuihcrre.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtvarkfjrp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gteakrikao.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtarbysrxo.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtlazqjesd.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtnuqrqnkq.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gtlckdkpzr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtaqbiozvs.html

JS:   toString() { return this.name; }
来源：http://hz.nanxinkj.top/gtutdncimh.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gtzewocmrj.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtcdzprztv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtkbqlxjpp.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtvkjsktcz.html

C#:   public override string ToString() => Name;
来源：http://hz.daria6918.cn/gteyzgltkq.html

[G13] 判断对象类型
来源：http://hz.ppjwa.cn/gtpzfrbnbz.html

Py:   isinstance(u, User)
来源：http://hz.zhongyouzk.top/gtzpfudpha.html

PHP:  $u instanceof User
来源：http://hz.gogol.net.cn/gtjotvzqnp.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtslkbwmwd.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtnrioybgn.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtbpnpokmk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuetiantiany.cn/gtckpjtdbu.html

Ruby: u.is_a?(User)
来源：http://hz.sxryk.cn/gtlqyqkhzz.html

C#:   u is User
来源：http://hz.chenjidiqi.icu/gtuwrvzwgs.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtuxhgltto.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yvedp.cn/gtbizewlrd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gtlwuaqpwj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtlflrhmqz.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtqzngqdpq.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtkxeemfod.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pycfn.com/gtrzjpgnva.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtajveqqcu.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtvxhmybwn.html

[G15] 枚举
来源：http://hz.birdmap.top/gtdnqxyfin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhaomingkeji.xyz/gthvntidwd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtzqvneiyt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtudywddfh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtjdwkdnub.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gtefepazxb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.birdmap.top/gteyminozi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nwbrower.top/gthijcbpwj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtmihtphag.html

[G16] 对象转数组 / 字典
来源：http://hz.hongshengwenyu.top/gtfknbirca.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtnigerirp.html

PHP:  get_object_vars($obj);
来源：http://hz.chenlongwang.top/gtcvrwottq.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtbpwkkell.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtvyzozvbe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gtvkutmiqr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.kuanghao11.cn/gtuhbvuzhy.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtnryxrpql.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.52xcode.cn/gtgrjdkaiz.html

================================================================================
来源：http://hz.yj202588.top/gtqwngihiy.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtmlvbimex.html

================================================================================
来源：http://hz.ivvv.top/gtebmjjbxq.html

[H01] try / catch 基础
来源：http://hz.zhongyouzk.top/gtcphqdfyl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtbuywopco.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtadpbojbi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtvunhovyn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtynzcfbik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.bjfxy.top/gtnaiwwxds.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtgxvztrku.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shangyingyoupin.top/gtqnsandtb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtvwnpfxsh.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtyjtwymjb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtsnbxpeit.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtjmfbjusg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtedcnfsrh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtwlkybdxz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtxivaozeu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jianghu66.top/gtsotqfbql.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtdckmzyyy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtqqiegeof.html

[H03] 主动抛出异常
来源：http://hz.fengsongda.top/gtsorigpqg.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtwglbcuhg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtlntyxoep.html

JS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtuhdtxemi.html

TS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtbeaaklhg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtiqejohkz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtzpjqmhze.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zdqjudy.top/gtleybeolb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtuxaebxkl.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtlepnibhj.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtifsdtmtu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtbcxvrcjr.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtnwkjeymz.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtqlaxrpet.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gtowtsnela.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuanzx.com/gtlvliwbeq.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtsvbgusef.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtlavafaww.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gtaxgekdpw.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtzhdffuad.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gtrrykwyyt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtuecqlpwe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gtniibzaqp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.mhx1999.top/gtzpfpcdjk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtsdmqyplg.html

Ruby: rescue ArgumentError => e
来源：http://hz.0kj1m.cn/gtxugowkbn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tianlin.xyz/gtpojfbxrk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258.top/gtwnbftcss.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gttsovbgyv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtnuuqtsya.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtfbegevny.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtvxpmhxpp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtgorioxai.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tian-w.cn/gtenetznku.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtlyhewjnp.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtmdqjnpef.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtqnlntkhc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtfadgrpmm.html

PHP:  assert($x > 0);
来源：http://hz.jianghu66.top/gtsreydrek.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtwcfrboug.html

TS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtmjsnonam.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtwwepmolu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtwjhzqlja.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.bjfxy.top/gtushauudj.html


<!-- 参考信息 -->