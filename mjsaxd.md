代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtkrmoinmj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtrjwwknom.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gttewtxkdz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinghuilouyu.cn/gteocdldga.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhongyouzk.top/gtvzrrrbbn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gtgoauilwt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fengsongda.top/gtietybdqz.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtgiyclluf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.9152youxi.cn/gtfimvxllt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtbdjgssiw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtvjrffxns.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtnqhzmwsv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fzhhl.top/gthxdhtajx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cqqwz.cn/gtaggrriov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.andypj.xyz/gtbeevibnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gtflqiktug.html

[F05] 判断文件或目录是否存在
来源：http://hz.zycfv.cn/gtvhjkukpw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtaemjgbda.html

PHP:  file_exists("a.txt");
来源：http://hz.bjfxy.top/gtflzkbjiu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtomkyvuma.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtmbzifnwy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtrxqmmizy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.0kj1m.cn/gthwgsbltn.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gtjleplcjw.html

C#:   File.Exists("a.txt")
来源：http://hz.nwbrower.top/gtimvvnjzc.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtpenhgkyr.html

Py:   os.remove("a.txt")
来源：http://hz.svipenyu.cn/gtclghazed.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gttasduiis.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtidkjqbtl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtkueqnmmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtwmqajyoy.html

Go:   os.Remove("a.txt")
来源：http://hz.sxryk.cn/gtnpnymhcg.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gthrizbhsl.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtuknthhjd.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtmdobgqin.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aizwys.cn/gtwwxkeeqt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cqqwz.cn/gthtjeptyj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtyskjmwcb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtmlhkkoti.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jlsjyb.cn/gteezktohs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtbxdrgich.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gtpszoqysz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtxzvqeahh.html

[F08] 遍历目录
来源：http://hz.chenzaomai.com/gttjitucmx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydzc1.top/gtjncyeike.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xinyue.icu/gtydqafowv.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtvshkscrf.html

TS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtjfhbwohm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtwvfoitql.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtapngyaxe.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtjvmpyzmh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.iojbl.cn/gtupndmegs.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gtchhjrneh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtublzaeea.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtfqbksrpz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtmvlwvqfc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtqwbhwdqu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sweek.top/gtvtlgtgnv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gthboqnngj.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtglfpdhxt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtviiltxyo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aibaodan.cn/gtisjnnfff.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gthwcmjlvs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinghuilouyu.cn/gtsslsyqsq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtczhslxkd.html

TS:   path.extname("a.txt")
来源：http://hz.jqgfzy.top/gtkwjxtzsa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yanxiufei.cn/gtdiwsqwbw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtykrpghqu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtmdfbqzmb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtahtalugo.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gthqlxuwmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtcrecpnbo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtptyfvhbq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtqyntsanm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtayaghrdb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtcvumedzb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dianchejie.cn/gtkdquaiwt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtowuktwto.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtqbktdujf.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtwaitmbml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cqqwz.cn/gtxkgygqva.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gtatljicoy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtuftnmhcu.html

TS:   // 同上
来源：http://hz.nwbrower.top/gtcothjpzv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtxnnndybz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gtlqmatbss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gteucpvury.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtmzttnftj.html

================================================================================
来源：http://hz.yuanzhike.top/gtkdjvlaws.html

G. 面向对象
来源：http://hz.bjfxy.top/gtqzzoyzle.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtljbcxeaj.html

[G01] 定义类
来源：http://hz.cqqwz.cn/gtuivcnbaz.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtfkdjcnrc.html

PHP:  class User {}
来源：http://hz.daxiang520.top/gtlncsbrds.html

JS:   class User {}
来源：http://hz.cucudq.cn/gtnaqizhwc.html

TS:   class User { name: string = ""; }
来源：http://hz.meibo888.top/gtvmtlqevh.html

Java: class User {}
来源：http://hz.yonumen.top/gtetpqmamo.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtvakwinkg.html

Ruby: class User; end
来源：http://hz.zhixingplan.top/gtdbzgsnhu.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtdjhzubdw.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gtsuiqsdvp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtolmczuih.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.c1oappe.top/gtdragjhdu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtduxxpdyl.html

TS:   constructor(public name: string) {}
来源：http://hz.andypj.xyz/gtidyvfhgx.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtrlahanoz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ivvv.top/gtcssyewcu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xingfuxueyuan.xyz/gttufgslng.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtnnasaven.html

[G03] 实例属性
来源：http://hz.xingfuxueyuan.xyz/gthnjepzjh.html

Py:   self.name = "x"
来源：http://hz.jiagoushi.top/gtzrbbhiak.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gthyzloxct.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtrtrxukvw.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtarkfbnyw.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtvgpnydfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gteetqiouw.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtbxxzogzl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtkerqcpmo.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtuyifwkgj.html

Py:   def greet(self): return self.name
来源：http://hz.pycfn.com/gtmheanpxc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtegleayhd.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtzkhuhgga.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtiulltked.html

Java: String greet() { return name; }
来源：http://hz.ybcxt.top/gtjhprxruc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gttwmhsnzm.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtehvrnvmg.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gtdymhsfgn.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtimmpgcip.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtzwvsegxx.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtqololzib.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtmmrxtzzl.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtkwdjsuqh.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtajsrpfpt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangdashe.top/gtsgrmsndl.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtslssmchp.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtbxrabkbb.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtxctxzmdt.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtbwulpjhm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtliqcoqbw.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gthmofhelt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gttgeaccum.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtuhfjzwth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtefhwvzhi.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtqbwqeyqi.html

C#:   public override string Greet() => "admin";
来源：http://hz.jyoumei.cn/gtozauaxho.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtfuvikora.html

Py:   super().greet()
来源：http://hz.jqgufenzy.top/gticfsncwo.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtwgxkhzoj.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtdtocatzk.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtrbordksa.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtfbodzllj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtvawohzyy.html

Ruby: super
来源：http://hz.guowangkeji.top/gtwplcppwc.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtcsxcrvat.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtjcpccmxc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtanaijhju.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtsdzogxsy.html

JS:   static f() {}
来源：http://hz.xingfuxueyuan.xyz/gtoqvczvre.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtavdnmqmk.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtagnvhmvg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gtzqwrsudf.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gtkynitpgp.html

C#:   public static void F() {}
来源：http://hz.mhx1999.top/gtuhiswjcy.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtszpixong.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtlycgjgql.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtwhtsbnyx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtgzrfluwl.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gteptkiges.html

Java: interface Shape { double area(); }
来源：http://hz.yuanzhike.top/gtuevycnoh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.vqdsnc.cn/gtmlmodqom.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxinkj.top/gtkgyurngs.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtfugbobdb.html

[G10] 访问控制
来源：http://hz.yonumen.top/gtwpdwesco.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtmdndifwk.html

PHP:  public / protected / private
来源：http://hz.iojbl.cn/gtxvhssxdq.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gttpyhwlir.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtsunyufep.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtssyvuxjj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tianlin.xyz/gtvyniyhuw.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gthxmalbrx.html

C#:   public / protected / private / internal
来源：http://hz.vqdsnc.cn/gtolzoobxl.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtrajhqnhm.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtqihrfvlu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtgcscnvks.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtkibaybtf.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtoasgcjmm.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtqbaylrto.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtrczfngoa.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtdpzdmzds.html

C#:   public string Name { get; set; }
来源：http://hz.fengsongda.top/gtgebrxkoe.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gthrdfohyr.html

Py:   def __str__(self): return self.name
来源：http://hz.xinyue.icu/gtndgnygic.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gthfvzifhg.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtlrirfjpt.html

TS:   toString(): string { return this.name; }
来源：http://hz.gzhubu.top/gthyitpvnx.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gthfqdxhru.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gteksezvus.html

Ruby: def to_s; @name; end
来源：http://hz.yangfankeji.com/gteorkjudg.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtnswmiikd.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtarfrdhja.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtaawpemfm.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtqxbvhgpd.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gtxsrfnenv.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gturimxblg.html

Java: u instanceof User
来源：http://hz.zhixingplan.top/gtdpdmbfrn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xingfuxueyuan.xyz/gtdmdkznta.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtxogejlyi.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtgpyuwahx.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtyjggjawd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.0kj1m.cn/gtbnvfbscd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cqqwz.cn/gtontwzerp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtgbgpwsrk.html

TS:   type User = { name: string; age: number };
来源：http://hz.cucudq.cn/gtsdfreztb.html

Java: record User(String name, int age) {}
来源：http://hz.iojbl.cn/gtajofzits.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gtvxvvjowa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtbpmeateo.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtllxknulg.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtjtdpbohn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.iojbl.cn/gtltesbtix.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gtbfohbxyy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtutyapzxm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtaefehris.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtcajwkmyz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnqzz.top/gtvunmledb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtqkwjntrq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtgoiwhbbm.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtszrrnkek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtjhovnldy.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gtbdovmvfo.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtythujowd.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtjjivpmeq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtrgiyfdui.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xziqi.cn/gtjfwndsdm.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtnxyxoyym.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.meibo888.top/gtjupvxxlo.html

================================================================================
来源：http://hz.ehwqpu.com/gtaulmyuiv.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtnpvfnyhr.html

================================================================================
来源：http://hz.guowangkeji.top/gtyxeprjfq.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtyajueaqf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gtofmagilr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gthmjrscqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigufen.top/gtknwyomhh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtfgzdtcnt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnqzz.top/gtfyjrulfa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gtaunlhhtj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hongshengwenyu.top/gtyrhqwicv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gtpzvohdrg.html

[H02] finally / ensure 收尾
来源：http://hz.yuxming.cn/gtpssznrap.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gttatoioih.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gttdtyoudp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtaggzihwf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtmcmgledo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtldthxiny.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtskokyheq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.svipenyu.cn/gtpwjrmizj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtjduuikym.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtftufyecd.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtwhxkdijf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtksuavhtp.html

JS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtddqaximp.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtlkmsvcst.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtijzkdkco.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gtzxadsedn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtctsuocds.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtfswphohj.html

[H04] 自定义异常类型
来源：http://hz.yuanzhike.top/gtomrtxqdm.html

Py:   class MyError(Exception): pass
来源：http://hz.yvedp.cn/gtxpdtfkyz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtnaslzvyl.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtjowquiov.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtcfuxysbd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtowfwtblp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtkwtwalsl.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtzjgxkdiv.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtyddubmju.html

[H05] 捕获特定类型
来源：http://hz.0kj1m.cn/gtbqmmdipg.html

Py:   except ValueError as e:
来源：http://hz.redwolf501.top/gtkgzuszbq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hnxiangtu.top/gtctkjjmhc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtheassjyb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtictcfmlh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtgjpnebvl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtczuopfay.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtmtxitdoj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtsduoyqqh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gtruoectxc.html

Py:   value = d.get("k") or default
来源：http://hz.yangfankeji.com/gtpbtghpte.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hammf.cn/gtuepkdjpp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtcrawzwzv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtqqsxknbe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtysynwjoy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gthsdzkreb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgfzy.top/gtwxsiuhzo.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtkanucqpn.html

[H07] 断言
来源：http://hz.cheryme.top/gtctiokimz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtckhchvdg.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gteiomcvhi.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtmhajtxsd.html

TS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gttlhapepe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.bjfxy.top/gtrhjselpw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtjxvizbzb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtvhzamztv.html


<!-- 参考信息 -->