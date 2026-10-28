代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.316326.xyz/gtwgxfbmqt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ppjwa.cn/gtzxmhdzet.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtipcghmmn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtljmrxefv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtepzeevir.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtlwyzlfzx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gttmjeqfwb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtoxbtnupz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gotoacloud.top/gtjoagemvz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtzvyebvio.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtxltfhqhc.html

[F04] 追加写入文件
来源：http://hz.ivvv.top/gtxncyosno.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtbgleoiuy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hysaishi.cn/gtalbtscff.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtrfjuudxf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtxmczenyj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtcgwclmnj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtwsfwqqlw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtpmxgeyom.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangtech.top/gtxymjvhyv.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtkxdgohom.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangdashe.top/gthvewsgqh.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtrhpdvgeq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtviyzpfmq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtxxnuztsq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtvocjjysa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtgnikwfae.html

Ruby: File.exist?("a.txt")
来源：http://hz.ybcxt.top/gtantieeph.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtephtxufq.html

[F06] 删除文件
来源：http://hz.yongpay.top/gtrjpfzkhr.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gthrczvcov.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtuayahjkc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtumyxhspn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtlleewfzy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtmqvznjvb.html

Go:   os.Remove("a.txt")
来源：http://hz.aibaodan.cn/gtweointaz.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtelhoivij.html

C#:   File.Delete("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtqtgrtrpz.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gthcbabvaq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtshnxiuae.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtvzatjezx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtitmvkaqm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtelglwstw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangkeji.top/gthdqsnpae.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenjidiqi.icu/gtubobfndv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gtbjfulxsr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtxbbgcypp.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtvfnyerhh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtafvpmbjo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtmvppukap.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gthibgaodi.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtgkkfjnpt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtkqnuqkdq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.kuanghao11.cn/gtksbnmmck.html

Ruby: Dir.children("dir")
来源：http://hz.fengsongda.top/gtfrymizxw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtngqjbvth.html

[F09] 获取文件大小
来源：http://hz.chenzaomai.com/gttyaxkyez.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gthqwcoozy.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtpiylvsya.html

JS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtzcixtwru.html

TS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtftumgjgi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtjxfeygoc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gttnahxaua.html

Ruby: File.size("a.txt")
来源：http://hz.xinyue.icu/gtiuongvke.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cucudq.cn/gtmflchorf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtolyryyro.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtevcombnx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtucqvctwu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtpkejbwbg.html

TS:   path.extname("a.txt")
来源：http://hz.vqdsnc.cn/gtswkgjqoy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nwbrower.top/gtyrdloyca.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gteovhmgwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtprmyltxh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtcrwwnctj.html

[F11] 复制与移动文件
来源：http://hz.hywenlv.cn/gtnoysqhhl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtamnknmfo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guowangkeji.top/gthllizlbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtuskruqpb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtxpjughaf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtkjjmhhyk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gtczwfodzt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtbgoehiir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtpbvegxid.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtiimlowvc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gthywkdrnu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtylhehnta.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtdevjnlsa.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtaizzexkl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gtcediemzf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtghfpwrhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtqdjvpdgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhiwuduotai.top/gtqtyxogfp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvjyfbtfq.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtclksqvvh.html

================================================================================
来源：http://hz.iojbl.cn/gtjkwqnsjv.html

[G01] 定义类
来源：http://hz.aizwys.cn/gtmvbnsehx.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtsivxogsa.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gtfrvrpuml.html

JS:   class User {}
来源：http://hz.zhijiandao.cn/gtitapjsmd.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtdharakjw.html

Java: class User {}
来源：http://hz.ivvv.top/gtonomzcim.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtesgjmdns.html

Ruby: class User; end
来源：http://hz.xingfuxueyuan.xyz/gtdqirtgae.html

C#:   class User {}
来源：http://hz.tanke756.top/gtnsqihxls.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtxttghwsd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtdyyulsnk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtbrouyvjd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sweek.top/gtgqcqueng.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtwyyclvsn.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtdxcuemhl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtytbhyhks.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hammf.cn/gtsvfxozsr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtggqhcqzl.html

[G03] 实例属性
来源：http://hz.dianchejie.cn/gtnrtpiqkx.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtswmphqju.html

PHP:  public string $name = "x";
来源：http://hz.fzhhl.top/gtiqmabjba.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtrcoeesyl.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtaoaagguz.html

Java: private String name;
来源：http://hz.jqgufenzy.top/gtwitgkxrp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtwmudfqle.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gteuovnojf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtfjggmkqg.html

[G04] 定义方法
来源：http://hz.haohaochexian.top/gtdwdzoess.html

Py:   def greet(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtxosugzdk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtlxxzoekr.html

JS:   greet() { return this.name; }
来源：http://hz.chenlongwang.top/gthbdmwfkx.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtukrupriw.html

Java: String greet() { return name; }
来源：http://hz.ppjwa.cn/gtumhtujlm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gteattptiq.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtssthemfz.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtamckzvjg.html

[G05] 继承
来源：http://hz.zhongyouzk.top/gtcnziajtc.html

Py:   class Admin(User): pass
来源：http://hz.52xcode.cn/gtqesyrcnw.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gtciptdusi.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gttvgttzyi.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtcrkcjzfd.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gtebynkihu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtqpvljqgs.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtjduhpctv.html

C#:   class Admin : User {}
来源：http://hz.shangyingyoupin.top/gtjburwpjg.html

[G06] 重写方法
来源：http://hz.svipenyu.cn/gtczmoomls.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtlgamnpos.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtyjkazaiy.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtikxgiyua.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtcruvzske.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtsadrrrmg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gthxjijouc.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtyiidahzz.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gtuomnaovz.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtezxwyjwf.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtjnopfbka.html

PHP:  parent::greet();
来源：http://hz.xingfuxueyuan.xyz/gtodkkdphx.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtxfnqvsfd.html

TS:   super.greet();
来源：http://hz.yj20258888.top/gtbhbwjuak.html

Java: super.greet();
来源：http://hz.sweek.top/gtetvuimuc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtilrdihka.html

Ruby: super
来源：http://hz.hysaishi.cn/gtvmfceppf.html

C#:   base.Greet();
来源：http://hz.guannengcc.top/gtoigcqhjy.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtdtaoerru.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtlgrbdngd.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtxpbyxidl.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtikzumvrz.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtjsbnzznk.html

Java: static void f() {}
来源：http://hz.ppjwa.cn/gtbyrvhewz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtufafagig.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtnakcsrhi.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtwxbsxufo.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtabeobdnt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtdjpukjxh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.kuanghao11.cn/gtfxgdhqxj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtikldltxq.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gtolnnybgz.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtnxeqyirh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtgjvpqvca.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnqzz.top/gtrvwffmos.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gtcpryqatx.html

[G10] 访问控制
来源：http://hz.xylfe.cn/gtgkazdgbw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtmpcauyyg.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtlobcupkp.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtdhkxumzb.html

TS:   public / protected / private
来源：http://hz.svipenyu.cn/gtasrksxpd.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gtaqjbekmc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dashuyun.cn/gtjiskuwim.html

Ruby: public / protected / private
来源：http://hz.mhx1999.top/gtuvttzagz.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtnfhujtnh.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gthmhnwybh.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtslckcfes.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtxnnltafr.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gthurgxjpe.html

TS:   get name(): string { return this._name; }
来源：http://hz.hongshengwenyu.top/gttjdqhlef.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtymslokwn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hysaishi.cn/gtovhsppyp.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtkgonfhmp.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtvueaanhu.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtygrlxhhl.html

Py:   def __str__(self): return self.name
来源：http://hz.yj202588.top/gtcbwmgcms.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtwtzuxryo.html

JS:   toString() { return this.name; }
来源：http://hz.9152youxi.cn/gtjltahqdw.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtkygbhxfv.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtfqpnxzuw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtlrtcshqv.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gtyqsfcmls.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gttqwbtrni.html

[G13] 判断对象类型
来源：http://hz.iojbl.cn/gtohozpuxz.html

Py:   isinstance(u, User)
来源：http://hz.ppjwa.cn/gtmgaqahje.html

PHP:  $u instanceof User
来源：http://hz.yuanzhike.top/gtsstnvfvx.html

JS:   u instanceof User
来源：http://hz.sweek.top/gtaugdfpqj.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gthzlxggge.html

Java: u instanceof User
来源：http://hz.jqgfzy.top/gtfzbjxvea.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtnebczwqd.html

Ruby: u.is_a?(User)
来源：http://hz.ybcxt.top/gtdlxhltun.html

C#:   u is User
来源：http://hz.smart0.xyz/gtldyqguhj.html

[G14] 数据类 / record
来源：http://hz.yj202588.top/gtymxrxgtu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gthuebtiia.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtbyrenrcn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gtrqiesvqq.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtfmudconn.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtjtanhyzf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gthxzgdrxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtghqymgpx.html

C#:   record User(string Name, int Age);
来源：http://hz.smart0.xyz/gtqyhubfct.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtsefadiqc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtzxumismc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtesvnhkrx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtlkridmwl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtaczhzmgg.html

Java: enum Color { RED, GREEN }
来源：http://hz.yangfankeji.com/gtwwbjvkaz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtlggpikhp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtcmdwzwsi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtffimbivc.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gtnhifslhx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtmefbycie.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtcretovzi.html

JS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtxhjxiqwr.html

TS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtcxwtouic.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yongpay.top/gtgnjgjuaa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtbjdtblaz.html

Ruby: obj.instance_variables
来源：http://hz.hysaishi.cn/gtlnlbmehk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtooqrebsr.html

================================================================================
来源：http://hz.fzhhl.top/gtjvckawky.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtmjiktlos.html

================================================================================
来源：http://hz.cqqwz.cn/gtcuhwtzgx.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtpfaahead.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtwmdshrna.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sysykeji.top/gtfbmwslgv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtdjqerbfr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gtvnvokobc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtckbpkslt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gthqhqnwau.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtrounqtbh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhiwuduotai.top/gtlajbxuml.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtbdslwota.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtywptects.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtrpoiquyz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtbwypwvgs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtonhuvwke.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gttupgdmcq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtntnbtawk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hfpthk.cn/gtkmindueb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.c1oappe.top/gtebdhnfoy.html

[H03] 主动抛出异常
来源：http://hz.hnqzz.top/gtvwtmxidx.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtypytfepm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtuvxczyhl.html

JS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtlheohxwl.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtoydisjce.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtoeqpypfw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtagfccypb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnxiangtu.top/gtarupwlfm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtugzxmbpx.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtodicgrnc.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gtbpvyzesh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gthwpvsmjv.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gttqejrscm.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtzkiscbjr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ybcxt.top/gtmwfiufew.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gthalyjmwa.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gtocknhubv.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtkiimchrg.html

[H05] 捕获特定类型
来源：http://hz.cashguo.top/gtihzvdeti.html

Py:   except ValueError as e:
来源：http://hz.yj202588.top/gtycqzahrr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gtusyorbae.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtkqhkrlhm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtbcryieeu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pengpengdd.cyou/gtaapmqdwd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtmejwglar.html

Ruby: rescue ArgumentError => e
来源：http://hz.hywenlv.cn/gtsjrshbua.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fzhhl.top/gtkbpvpnfc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gttrpryvjy.html

Py:   value = d.get("k") or default
来源：http://hz.xuetiantiany.cn/gtiraxvayw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.haohaochexian.top/gtznznugjn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtikvgyydc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtimwztmmb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtanznzbfr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtpsrcvljk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sysykeji.top/gtzcwrevbx.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gttzznkitb.html

[H07] 断言
来源：http://hz.chenlongwang.top/gtmliefmxi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.c1oappe.top/gtdyvdndpw.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gtlevppjlx.html

JS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtdpqdgnal.html


<!-- 参考信息 -->