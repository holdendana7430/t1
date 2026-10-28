代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtiitsikii.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtpfotpzwr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtrhkkdhox.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtushaaasc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtivzbctaf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gtygqhkwcf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gttudiqrtq.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtacrbdjlb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtznplevcg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtgyxpmjdl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtyxzdpvke.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gthpblgkeh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinghuilouyu.cn/gtcrexexyk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hammf.cn/gtzvhxdolr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtacsgqtsl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cashguo.top/gtpeidblni.html

[F05] 判断文件或目录是否存在
来源：http://hz.daxiang520.top/gtoraeapdm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj202588.top/gtlzkpyjdp.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtvyvohkge.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtxjzypamm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtivkmnemw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtjsynrneq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.0kj1m.cn/gtydfnueqv.html

Ruby: File.exist?("a.txt")
来源：http://hz.shangyingyoupin.top/gtxmdttucq.html

C#:   File.Exists("a.txt")
来源：http://hz.zhongyouzk.top/gtzxuavdmb.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtoirzigkl.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtjzpuhokm.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtsrqnstpj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtvarhvwde.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtnmczasbi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtjwydzcxa.html

Go:   os.Remove("a.txt")
来源：http://hz.sxryk.cn/gtouegwtyd.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtsgjuqlqf.html

C#:   File.Delete("a.txt");
来源：http://hz.aibaodan.cn/gtrmivspkh.html

[F07] 创建目录（含多级）
来源：http://hz.0kj1m.cn/gtkaczrgzz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gthdhfpytw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtfhnhksek.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtiuvbixeo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtwjieikuq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtqnydwnxr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtliwbvfch.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuanzhike.top/gtbqhbyovv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtdfrjjblu.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtputanowt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtwybbsnqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ppjwa.cn/gtlxcrbnju.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtvdkluzfh.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtqtuwpyrb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gteyhpjgtr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtcawdwsrl.html

Ruby: Dir.children("dir")
来源：http://hz.smart0.xyz/gtczchzqos.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gzhubu.top/gtlgusyqub.html

[F09] 获取文件大小
来源：http://hz.c1oappe.top/gtdpdpmmux.html

Py:   os.path.getsize("a.txt")
来源：http://hz.0kj1m.cn/gtsygdyiew.html

PHP:  filesize("a.txt");
来源：http://hz.chenjidiqi.icu/gtutzrwphi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtprzfwiwv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtoxhzogrw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtfikcuexs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtjjxhdbfb.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gthzgcmrad.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtihkwszmm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtgiwhkgdw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gthwvtksnt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtacbzejyy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtgzzbplup.html

TS:   path.extname("a.txt")
来源：http://hz.dianchejie.cn/gtujbjlsmi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gtblvdfcns.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gotoacloud.top/gtrxaahizq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtqstughva.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gttcqheofh.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtossukwsm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtuzkrvfrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shuidangran.top/gtllfucupg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtmsdqkpwu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtwqvdztmu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtltculiot.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guowangkeji.top/gtrvwybxka.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtdwtvbvnh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtzallrdzz.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtjbbjpazo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgfzy.top/gtrrjijqjt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtxfcvdkbz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ybcxt.top/gtqqlwwjps.html

TS:   // 同上
来源：http://hz.birdmap.top/gtdbzvemmv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cashguo.top/gtbuqddaos.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gtxiqiistw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtvpfqeoqd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtwenprmkf.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmirpifeq.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtdzolqyoo.html

================================================================================
来源：http://hz.shuidangran.top/gtdlctwapi.html

[G01] 定义类
来源：http://hz.yuxming.cn/gttwcxvggc.html

Py:   class User: pass
来源：http://hz.tanke756.top/gtiebgmylx.html

PHP:  class User {}
来源：http://hz.havefunace.top/gtyndjxahg.html

JS:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtvsbttopv.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtnrtlrxwg.html

Java: class User {}
来源：http://hz.andypj.xyz/gtuzvhsqse.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtlvzenbfq.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gttyxnuvwb.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtfklkyecc.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtleganimc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtycsjxuuk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shzxlz.cn/gtksxfjqdk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtaqrhghkj.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtnibfnuoe.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtnkhvubkl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gotoacloud.top/gtfuaohsdu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtuynwnylc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtwwsqzmzz.html

[G03] 实例属性
来源：http://hz.yj20258.top/gtmmpsefsw.html

Py:   self.name = "x"
来源：http://hz.ivvv.top/gtmbumfvuu.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtjymufcqd.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtwlmfpevv.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtkruuvrhe.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtdqcrgiqq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gotoacloud.top/gtudgwmzho.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtfhwzkiyc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtdwmwbbji.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gtqqufmedh.html

Py:   def greet(self): return self.name
来源：http://hz.aizwys.cn/gtfzzarxfj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gthuxoqlfu.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gtotpwqetq.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtaeuymprh.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtphqixyya.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtiojtaola.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtstxawufq.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258888.top/gtguxwoufp.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtogsamfxp.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtzatbonqr.html

PHP:  class Admin extends User {}
来源：http://hz.yj202588.top/gtranaglsi.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtvuzojbcc.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtsitkeppu.html

Java: class Admin extends User {}
来源：http://hz.yj20258.top/gtfgkxbpnf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yonumen.top/gtszyidkfp.html

Ruby: class Admin < User; end
来源：http://hz.chenzaomai.com/gtxfxiatxe.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtbaqgbltc.html

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtzbkdlqjw.html

Py:   def greet(self): return "admin"
来源：http://hz.cheryme.top/gtarmfiolz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtybhpyhpc.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtxwbbavxs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtqtairllu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtyljnqgxw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtdclhqdqi.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtrhywifro.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtwiuzmbxi.html

[G07] 调用父类方法
来源：http://hz.redwolf501.top/gtkhhajaum.html

Py:   super().greet()
来源：http://hz.cheryme.top/gtlhqzzxcg.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtkgrkweeq.html

JS:   super.greet();
来源：http://hz.chenlongwang.top/gtlmkerwii.html

TS:   super.greet();
来源：http://hz.chenlongwang.top/gttskkyhsp.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtkiqlvsti.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gtipdqeaks.html

Ruby: super
来源：http://hz.hysaishi.cn/gtpknvbtdj.html

C#:   base.Greet();
来源：http://hz.fengsongda.top/gtjbspmdfx.html

[G08] 静态方法与属性
来源：http://hz.c1oappe.top/gtyeqjsfnh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtdkbxihyl.html

PHP:  public static function f() {}
来源：http://hz.ydzc1.top/gtryrmeyic.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtzdzctlbh.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtdjagoxer.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtsryhnosy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtczuekvlw.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtxgpajgaf.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtcwtpqyom.html

[G09] 接口 / 抽象类
来源：http://hz.cqqwz.cn/gtjhdectki.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtmdoaseru.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sweek.top/gttbssvvul.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuetiantiany.cn/gtzpbhnaxi.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gtlchggkck.html

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtvlgmpumf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtcxwuaslb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtntwbfrpp.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtrejzgruy.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtfwmhrjaj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnqzz.top/gtdhqdciwz.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gtyqamrojh.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtczymxihv.html

TS:   public / protected / private
来源：http://hz.zycfv.cn/gtoulbtatj.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtotjeqxqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtzvnznuxu.html

Ruby: public / protected / private
来源：http://hz.316326.xyz/gtnhcesjny.html

C#:   public / protected / private / internal
来源：http://hz.jinghuilouyu.cn/gtsgrlendm.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtlusuuktx.html

Py:   @property 与 @x.setter
来源：http://hz.cashguo.top/gtckywdrxi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtcikjgtor.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtbginyqsx.html

TS:   get name(): string { return this._name; }
来源：http://hz.hongshengwenyu.top/gttebikgfa.html

Java: public String getName() { return name; }
来源：http://hz.jiagoushi.top/gtsvrqffcm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jiagoushi.top/gtjbygertw.html

Ruby: attr_accessor :name
来源：http://hz.gogol.net.cn/gtwlxvwlpo.html

C#:   public string Name { get; set; }
来源：http://hz.jyoumei.cn/gtjsenxggu.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gtkwhlusbv.html

Py:   def __str__(self): return self.name
来源：http://hz.chenzaomai.com/gtyexumgel.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtuetpmqyf.html

JS:   toString() { return this.name; }
来源：http://hz.guowangkeji.top/gtpchyqymo.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtdiysxntb.html

Java: @Override public String toString() { return name; }
来源：http://hz.9152youxi.cn/gtgdjpefwk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtmkrozvme.html

Ruby: def to_s; @name; end
来源：http://hz.sysykeji.top/gtdhnprbra.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtocindiwr.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtinutclla.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtdjovlmrz.html

PHP:  $u instanceof User
来源：http://hz.svipenyu.cn/gtytebwway.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtthihegmo.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtqgwcwrjl.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtvvnawpla.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gttpzputcg.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtyrjgquwt.html

C#:   u is User
来源：http://hz.fzhhl.top/gtvarnduxg.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtpnhvntvy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtbojlcinf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yueranfly.top/gtumtlzrvz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtkispefnp.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtldmffihr.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtzccecorj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gthhkltngv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtyqabrbhe.html

C#:   record User(string Name, int Age);
来源：http://hz.xuanzx.com/gtsbfthfke.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtfgcbpkcl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tanke756.top/gtofypbgct.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtnzqwmjzs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gtivynipke.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtvbcutkdo.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtghppckwy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gtzqygqyrw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtuzruyrkl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtsrkltkvh.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gtceiofhgj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtyrrzbquz.html

PHP:  get_object_vars($obj);
来源：http://hz.316326.xyz/gtiicnbvlt.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtwkvlbjjz.html

TS:   Object.entries(obj)
来源：http://hz.meibo888.top/gthljfgium.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtnpxbhqqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtzskyvzgy.html

Ruby: obj.instance_variables
来源：http://hz.ywan-chungtsiang.top/gtvxdbwiko.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zdqjudy.top/gtirccsalt.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfjgrmdjw.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gtqwqfbjhx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwwbpruvt.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtjuymivzs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtwwmzujmw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtoqvdfadu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtmbgitxcj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtbapuuxun.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gtxspbutan.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gteufffbwb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.c1oappe.top/gtwtqihcnp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtvkufnevw.html

[H02] finally / ensure 收尾
来源：http://hz.guannengcc.top/gtrenbbode.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtwvfgqwtk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtthhliqez.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtcdzgsvss.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtfrluatad.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtcthackyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtbgrncicq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtonpmfjym.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtvysfqfdz.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtbzepmsqi.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinghuilouyu.cn/gtqydaxhvc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtuuyalcjo.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtqbxkfyoe.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtbfawtzjw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtduediyna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daria6918.cn/gtatibcuwq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtceduknfn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtrsfbehmk.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtnitvwrgi.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtpizfsetk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtqsycfeuj.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtggllzrnv.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtnmiyataz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtfrlvilht.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangtech.top/gtagqfpcdi.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtqeifiufm.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtrokrtzxx.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtukzazdbq.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtaggyrxmd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtmwjarxps.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtfmyuapwz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtchmmrhmk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtpodffauq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtlfecmzln.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtoywyggix.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtxiufwxkt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtypgkefac.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gthdjioetl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtvawllgdt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtwbymaziw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtgehqtdqy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtbslhsjve.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuanzhike.top/gtpoixibfl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gttdjdbydw.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigufen.top/gtuegcarnp.html

[H07] 断言
来源：http://hz.tianlin.xyz/gtdfrqmkzq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtbycegloj.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtwtwpibtj.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtcqkieiod.html

TS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtexzwvvmd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gtxnvxwaaz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtdqkldswq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtfuwqcjmd.html


<!-- 参考信息 -->