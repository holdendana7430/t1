代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigufen.top/gtpmtcublm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtbwsqvbpx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gthjzxjery.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtzacfbcru.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenzaomai.com/gtoyocszmv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gtrvcynyrb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtfjojatcj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtrwhajmue.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gttizdutjs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.redwolf501.top/gtcbiktrfr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtuqrirwgf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtpavpopmc.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtiwbhwdrh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtcwgjwswp.html

PHP:  file_exists("a.txt");
来源：http://hz.xziqi.cn/gtvttqfcbw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtycygzfny.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtxlucswxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtoeggflpt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gthrwxeomd.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtpfogbqne.html

C#:   File.Exists("a.txt")
来源：http://hz.gogol.net.cn/gtxdsngmus.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtswfulmbo.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtijnzbrst.html

PHP:  unlink("a.txt");
来源：http://hz.jianghu66.top/gtrwoxzckg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtxkqdtjne.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtecwzafqu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtkgazxsvf.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtwtxkmtmi.html

Ruby: File.delete("a.txt")
来源：http://hz.ydjk.org.cn/gtibysuyux.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gtlbltlzfo.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtuflvsbuh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gtcwkpmvdz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtqldapgrp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtibbtwdkb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gttglrgqao.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydjk.org.cn/gtfagtsjvf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gttezuxsql.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtdotphlje.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gtgdynbeek.html

[F08] 遍历目录
来源：http://hz.ehwqpu.com/gtghdiumsl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtqdncbgkz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guannengcc.top/gtbzkagruz.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtxbsbfbwd.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtmoqvyabn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gttyvlywtn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuxming.cn/gtofwngxpq.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtgzrwvimh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtvslynptl.html

[F09] 获取文件大小
来源：http://hz.dianchejie.cn/gttoujwxvj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkearrbdc.html

PHP:  filesize("a.txt");
来源：http://hz.jyoumei.cn/gtdnidgrog.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtdmukdirj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtatemoyti.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtyfdngpxz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenzaomai.com/gtygrpcejp.html

Ruby: File.size("a.txt")
来源：http://hz.shzxlz.cn/gtscbautqq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuetiantiany.cn/gtoyxgorov.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtremrnryb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtgcazpmkg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtwioddyjs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtnzwmwyou.html

TS:   path.extname("a.txt")
来源：http://hz.fengsongda.top/gtzzuatttp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtfvgvymht.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sufxvd.cn/gtfbvfdvzs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gthqppwgjm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gzhubu.top/gtyeqxhosp.html

[F11] 复制与移动文件
来源：http://hz.jinghuilouyu.cn/gteuehhkut.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtjjlnlysb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtnpiciyqc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtnksdcobm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtjirepnfp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.pycfn.com/gtxhgmyrqr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtjbdnhbdv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtwoyuedmn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtfascnpyh.html

[F12] CSV 读写
来源：http://hz.guowangkeji.top/gtfhpuzjcs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtwmlktqyd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtketkrtwb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gtqzjtbbes.html

TS:   // 同上
来源：http://hz.hammf.cn/gtjmzdddxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cashguo.top/gtmzcweloj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtaetdggps.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.kuanghao11.cn/gtfwkyiaaz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ivvv.top/gtmfpqalzo.html

================================================================================
来源：http://hz.dianchejie.cn/gtbvvhnons.html

G. 面向对象
来源：http://hz.hnqzz.top/gthwdwugfk.html

================================================================================
来源：http://hz.yueranfly.top/gtxfkdvdrc.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtpfeqioqf.html

Py:   class User: pass
来源：http://hz.dashuyun.cn/gtzlxgplma.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtwpaxoaog.html

JS:   class User {}
来源：http://hz.ybcxt.top/gtznjvwary.html

TS:   class User { name: string = ""; }
来源：http://hz.daria6918.cn/gtesxtefbf.html

Java: class User {}
来源：http://hz.ppjwa.cn/gtulgesugw.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtxqlkppfm.html

Ruby: class User; end
来源：http://hz.quarkkingdee.top/gtbukwlmap.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtbveededl.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtwvhivsvm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yangfankeji.com/gtblfprcus.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtqdrgqkwx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtqtkoxnjf.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtbyrrdrgd.html

Java: User(String name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtsqqzbepl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtzzrcmmho.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtfdlqkpgt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gtmxrxqlnr.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtvdutfqqe.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gtxbmgpbhd.html

PHP:  public string $name = "x";
来源：http://hz.jyoumei.cn/gtdiimxoau.html

JS:   this.name = "x";
来源：http://hz.c1oappe.top/gtezauazll.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtvntkfexe.html

Java: private String name;
来源：http://hz.c1oappe.top/gtngijntjb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtvckxopok.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtetsxummp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ivvv.top/gtyctlitxf.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtzdassuwd.html

Py:   def greet(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtuwlgwwdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.birdmap.top/gtuuctlsjv.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtjovekuof.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtlvclxhws.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gtjnvsutcb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtsnqvniat.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtcdbazeux.html

C#:   public string Greet() => Name;
来源：http://hz.daria6918.cn/gtcypbswbx.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtkbchzpkc.html

Py:   class Admin(User): pass
来源：http://hz.ivvv.top/gtvvboaosa.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigufen.top/gtsidoeaha.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtivdllvia.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtzwhbpkmn.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gtcprehglv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.0kj1m.cn/gtrydovair.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtwczbmbbf.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtvwcyrzuy.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtqghihpjg.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gtxaaknytp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtfhyfyvhf.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtdwxtngge.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtadljsgvx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtjbuoccdi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuanzhike.top/gthtzfcyva.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtuucplzcl.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtkqyjwsbx.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtrvsztizy.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gteqfvzgur.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtoktnuzis.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gthzzdzvdu.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtbyfiafwg.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtyyvotxuv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtinzwrwyv.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gtyvctlftj.html

C#:   base.Greet();
来源：http://hz.tanke756.top/gtrvjxnlrl.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtbepvamad.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtdjyobjzj.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtxvecfkva.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtryvefqrx.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtzsbrwxlf.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtdvidihnu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.feifeiyinyue.top/gtgkgsapvv.html

Ruby: def self.f; end
来源：http://hz.smart0.xyz/gtlfznrncp.html

C#:   public static void F() {}
来源：http://hz.nwbrower.top/gttflwcxzs.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gtsbdsijxr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tanke756.top/gtgiwvnhvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtaykqsbzx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jlsjyb.cn/gtiatiqvpu.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtvdsoxrto.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtmgezpxgw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtknhlfqio.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ehwqpu.com/gtjhmkpzuj.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtqcfinqbe.html

[G10] 访问控制
来源：http://hz.tanke756.top/gtgyiebuug.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zycfv.cn/gtuumqgyev.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtuaqjtgxl.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtskroftwu.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtsxrfbnui.html

Java: public / protected / private / 默认包级
来源：http://hz.sxryk.cn/gtenxkehiv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gtljathwog.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtxasxsxay.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtoawafvsk.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gtbdpklddf.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtvchlhvta.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtqturyhxb.html

JS:   get name() { return this._name; }
来源：http://hz.zycfv.cn/gthqkdlfcs.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtamwuabni.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gteyaeocbk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtzelxhjhx.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtvgnyhjmg.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gtiaeaycnk.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtanlrqrqa.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gtrwonnmfj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtpnbetunz.html

JS:   toString() { return this.name; }
来源：http://hz.jianghu66.top/gtouogeflp.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtlhogogwh.html

Java: @Override public String toString() { return name; }
来源：http://hz.feifeiyinyue.top/gtmqfreixy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.smart0.xyz/gtnwptqkzg.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtuqrrgycl.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtluliyhcs.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtpdhmevjp.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gtftwtdoat.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtjifktdcw.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtlzqgnvwl.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtbttumwhv.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtmtsoeval.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gttupupeeg.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtxzwoooar.html

C#:   u is User
来源：http://hz.ybcxt.top/gtizhjjuyj.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtzcndsbot.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtjvhysqrg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.haohaochexian.top/gtcxvbbigy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtmjxuufmg.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtjqidsofp.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtwjeqgfib.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dianchejie.cn/gtfqcehfus.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fzhhl.top/gtbefehdin.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtodatijoa.html

[G15] 枚举
来源：http://hz.xylfe.cn/gttoglzuar.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtsnuypopb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gttltwhrft.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gttzcnehie.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtgpsiyugp.html

Java: enum Color { RED, GREEN }
来源：http://hz.52xcode.cn/gthdvdckxd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtpupidqcw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtrbxadwjc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtsujahdrr.html

[G16] 对象转数组 / 字典
来源：http://hz.sufxvd.cn/gtikhiekyu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtewsjhhwk.html

PHP:  get_object_vars($obj);
来源：http://hz.ybcxt.top/gtzrtrdwdl.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtshztomvs.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtxervzhvs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtkjfjipzc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtwclfgeve.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtxqfkvohc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtvmzajnnj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsioducsj.html

H. 异常与错误处理
来源：http://hz.yangfankeji.com/gtgglgnjgd.html

================================================================================
来源：http://hz.yj20258888.top/gtpmkpvtpm.html

[H01] try / catch 基础
来源：http://hz.zhiwuduotai.top/gtfnrqgxae.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tianlin.xyz/gtmvamfqlt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtopyovuni.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtckuvbpky.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenzaomai.com/gtyjjpxovm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtzhungwao.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtxatguovr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtzmzsqrpf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cqqwz.cn/gtvazrflgz.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtsaojfuuj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtnxuexkhh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtnrxbuvri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtfoirehfw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtabdtehnu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtlfqmpgbm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtpxyajqfm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtpiahekvy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtnzragquc.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtzindqskp.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtlmdkzjhb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtukipstpi.html

JS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtkykxnlup.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gthqfpniqi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtplplboaf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtavkaczjs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtssoxslkh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtthcfvcbz.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtfflbbgkp.html

Py:   class MyError(Exception): pass
来源：http://hz.hnxiangtu.top/gturxvoxva.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtslvdvrnh.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtxmrjecko.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtblyprdmo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtnasmhrpu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtaxbridjn.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtillkxssh.html

C#:   class MyException : Exception {}
来源：http://hz.hnqzz.top/gtuasrqcxe.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtnpqybabm.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtxwmtezyw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gtmuuseflh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtznmwhvgc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtdvtuhyjb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtnerbwqpf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gtmuopulfe.html

Ruby: rescue ArgumentError => e
来源：http://hz.316326.xyz/gteabvbcsn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhoulong.xyz/gtftvdvqke.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hammf.cn/gtuckmrpvm.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gttujvdbyl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtuumtnwch.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtpqpaxnbn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtweyhxrrx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cqqwz.cn/gtfnxkdmjc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtvotqvvxl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gtbqqqnjnu.html

C#:   obj?.A?.B ?? default
来源：http://hz.aizwys.cn/gtqxuzuoce.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtcwwappdp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtksqcrfqi.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtmvrqdibn.html

JS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gthytqxzkh.html

TS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtrxrbirfw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gtwlayaoty.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtfvlzplhh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtcnttpixv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtlmgmzqas.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtxbpvgseo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtzjwibmyd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnqzz.top/gtxknahokv.html


<!-- 参考信息 -->