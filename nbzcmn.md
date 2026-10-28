代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtphrjpzxp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtmnbfwlai.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtkpwfucxj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258888.top/gtlridzggi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtcegwuqif.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gtaiqkdknm.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtmkmtmpdm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtxqbjmoxo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtnequuosc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtegsuzpgg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtwitoilyv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gtgflxbuui.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gtaoermmev.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cashguo.top/gtqoazztnb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtabibkymo.html

[F04] 追加写入文件
来源：http://hz.zhaomingkeji.xyz/gtlydljuok.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtfnitvqmj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtupifoqht.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtgrsgdxfu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtokoqeldh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtvivdmpim.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtyywamzgp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hongshengwenyu.top/gtpgdmfwfb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtogjkigys.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnqzz.top/gtlhepxnpf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gtpnqcqrlw.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gtghikidwz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gttdhdhaii.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtsejwzkir.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtdqcosdfn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tanke756.top/gtwhvwyden.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtnfivpllo.html

C#:   File.Exists("a.txt")
来源：http://hz.ydjk.org.cn/gtindbbmjb.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtnzyjyjsu.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtzycvdkll.html

PHP:  unlink("a.txt");
来源：http://hz.yuanzhike.top/gtielzuvid.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtcfipfegh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtoaluwgvd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtkwfigisi.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gtyosfsyck.html

Ruby: File.delete("a.txt")
来源：http://hz.iojbl.cn/gtpcqsrivo.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtuvzhedsk.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtbpttnwbb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gthrudjgva.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtemxdpuyn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gttioqcwrl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtnyaccniy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gotoacloud.top/gtsllngjvs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shzxlz.cn/gtirwmcmrh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.andypj.xyz/gtslzeifle.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.havefunace.top/gtajdkpabt.html

[F08] 遍历目录
来源：http://hz.yangfankeji.com/gtzeatykfv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtxfwurnhg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuetiantiany.cn/gtyrnaunpe.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtfacctbyj.html

TS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtjmgnryej.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shuidangran.top/gtiatzsrbw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xinyue.icu/gtmegmkfxj.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtqzgrpieo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtgwqhlwmh.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtofuuuwkd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gttjuvkkrd.html

PHP:  filesize("a.txt");
来源：http://hz.sysykeji.top/gtwhruryoj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtfgbozdky.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtlevkuvau.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtsfxrdgiq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shuidangran.top/gtvbaioxxp.html

Ruby: File.size("a.txt")
来源：http://hz.ppjwa.cn/gtbjipqkfl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258.top/gthaapjzgf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtfzvbjgrs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gthndxpdoz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtadmanllh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtkscltxni.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtwdrsymgn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jyoumei.cn/gtiiiqfsuq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtqqnwvlpy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gttevpurpw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gttpwrdnge.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtbhaemmsk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gthpmsemoh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtwfijfhvh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtmlooexsg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtqrzzzzcn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtzckvoxck.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.316326.xyz/gtvwfdufjq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtbvnehfmb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenjidiqi.icu/gtnbxittlw.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtxqljnaum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fzhhl.top/gtrsjojooh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtaqascwtk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinghuilouyu.cn/gtmnjyfygq.html

TS:   // 同上
来源：http://hz.cdnleiting.top/gtpyigvdrr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cashguo.top/gtgcentbhn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtefgvfngc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ppjwa.cn/gtogoyzlsp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ivvv.top/gthvmigsdo.html

================================================================================
来源：http://hz.wangdashe.top/gtjqqcemkx.html

G. 面向对象
来源：http://hz.ehwqpu.com/gtxafkpkwm.html

================================================================================
来源：http://hz.guowangkeji.top/gtgkhkwzny.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtvdxjjsiw.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtbnbudtfq.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtaulficyk.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtxafdfqav.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtceuoufhh.html

Java: class User {}
来源：http://hz.yangfankeji.com/gtqugryxzq.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtwtidynje.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtrvwomibf.html

C#:   class User {}
来源：http://hz.jqgufenzy.top/gtvhlanjlz.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gttulofywp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnxiangtu.top/gthjbnvhjb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gthpdmzwqq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtqquxdbhd.html

TS:   constructor(public name: string) {}
来源：http://hz.zdqjudy.top/gtvnsmacbi.html

Java: User(String name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtnxyvbnbz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hywenlv.cn/gteugpjaob.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gthxtpzrfp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ehwqpu.com/gtrbknurzg.html

[G03] 实例属性
来源：http://hz.svipenyu.cn/gtjkcegpmz.html

Py:   self.name = "x"
来源：http://hz.zhaomingkeji.xyz/gtkuqkohbo.html

PHP:  public string $name = "x";
来源：http://hz.shangyingyoupin.top/gtodesivut.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtalbnvpbu.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gtmvtjczug.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtdongfszu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtjishyqwr.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtmbiatujk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtaowvusod.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtnkmgzmir.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtzfodohif.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtfiafitdj.html

JS:   greet() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtqlxyosvx.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtwoerxgku.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtuixhfjcn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtjywmkpyv.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtvpjpsyxp.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gttorjshlv.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtxmvamsfb.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtlxhibaub.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtreanujjg.html

JS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtffsfhhyn.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gttfnpdbkx.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtdzldhmhu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhijiandao.cn/gtsilgeawv.html

Ruby: class Admin < User; end
来源：http://hz.jinyuanbaomall.cn/gtfqogccbi.html

C#:   class Admin : User {}
来源：http://hz.jlsjyb.cn/gtaxpiuywc.html

[G06] 重写方法
来源：http://hz.0kj1m.cn/gtpdlbnqcl.html

Py:   def greet(self): return "admin"
来源：http://hz.shangyingyoupin.top/gtrxltsydl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtvaxmrljv.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtttapycrp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gthokejhte.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtgrlwwsff.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtggbtuavh.html

Ruby: def greet; "admin"; end
来源：http://hz.bjfxy.top/gtlbhvoacz.html

C#:   public override string Greet() => "admin";
来源：http://hz.gogol.net.cn/gttzrqgaam.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtuyyieitn.html

Py:   super().greet()
来源：http://hz.yonumen.top/gtfykbnral.html

PHP:  parent::greet();
来源：http://hz.xinyue.icu/gtblajzadm.html

JS:   super.greet();
来源：http://hz.daxiang520.top/gtuulaafpf.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gtuzhgkjfa.html

Java: super.greet();
来源：http://hz.shzxlz.cn/gtmthpdgae.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtnqhwlsnk.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtlezxfzrs.html

C#:   base.Greet();
来源：http://hz.zhiwuduotai.top/gtstuhprlm.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gtmiesjcps.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtrpqfwztu.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtdyspgjor.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtlejdurji.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtxfasetth.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtdtgdxmeh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtgphgirkf.html

Ruby: def self.f; end
来源：http://hz.guowangkeji.top/gtuztspkml.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtujemkmxc.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtigrprfci.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtznlmhtsj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtopgchnqf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtjzvucdah.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtmftnrmcc.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gttnxijiqy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtgzfekmee.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zycfv.cn/gthpxjzimk.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtplskkztr.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gtniqsntss.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtfjswdgpv.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtxmhuttwh.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtpcnfdusq.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtveihgicp.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtvddgmlgm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtadcqkuyc.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtagbbcsjv.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gthrzcuiyf.html

[G11] getter / setter
来源：http://hz.zhijiandao.cn/gtyiujkxql.html

Py:   @property 与 @x.setter
来源：http://hz.birdmap.top/gtiishirga.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtimkyxvft.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gthlwfolbt.html

TS:   get name(): string { return this._name; }
来源：http://hz.xylfe.cn/gtrlhnqkhi.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtdhgnenge.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gthvrkppwk.html

Ruby: attr_accessor :name
来源：http://hz.meibo888.top/gtotdgaqfu.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gttgahftmy.html

[G12] 对象转字符串
来源：http://hz.hfpthk.cn/gtnwwqrrdr.html

Py:   def __str__(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtfhssfdfv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtpyeaoslh.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gttdwkqyye.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gtzedcoiwb.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtqzehujta.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtxlbacccf.html

Ruby: def to_s; @name; end
来源：http://hz.wangdashe.top/gtgziiciyy.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtxvwrbtrh.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtjiluyaft.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtpiimbdxb.html

PHP:  $u instanceof User
来源：http://hz.yvedp.cn/gtmvfiucdj.html

JS:   u instanceof User
来源：http://hz.hysaishi.cn/gtvkzpobrk.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gtmzqdsfqq.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gthaxxokcr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.52xcode.cn/gtvmzofbyz.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtkalkhntl.html

C#:   u is User
来源：http://hz.zhaomingkeji.xyz/gtmmbynlme.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtrmeeqvqy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxuanxn.top/gtmubhkraw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtkmoktbdp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtunlraejg.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gtnefqblko.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtnjxxmqht.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shangyingyoupin.top/gtvlcjrvsl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tianlin.xyz/gtvuaahmrr.html

C#:   record User(string Name, int Age);
来源：http://hz.gzhubu.top/gtiqnwgbal.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtxeysgobs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtxdxrxzqq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gtclcpsnvo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.316326.xyz/gtizvhthva.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gthnhyqvfj.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydzc1.top/gtpmqbebvj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gtmczpixbr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ybcxt.top/gtcepdsvlu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtqoygzqma.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gtiajakprh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cqqwz.cn/gtgtaiwfnw.html

PHP:  get_object_vars($obj);
来源：http://hz.shangyingyoupin.top/gtdazvayjm.html

JS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtkmlhmmdl.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gttxelempa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtoketqpot.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtugqybgec.html

Ruby: obj.instance_variables
来源：http://hz.fengsongda.top/gtztdzppud.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtljvrtjxe.html

================================================================================
来源：http://hz.jqgufenzy.top/gttcouytpk.html

H. 异常与错误处理
来源：http://hz.ivvv.top/gtzumwsvin.html

================================================================================
来源：http://hz.gogol.net.cn/gtjyiwkedx.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtbwzevkac.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtztxduuyf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhongyouzk.top/gtwgrftgff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtorugyaif.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj202588.top/gtelsjveaw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj20258.top/gtfjyilqww.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtrekftdyg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtqmzplmoc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gthitiyrtz.html

[H02] finally / ensure 收尾
来源：http://hz.pengpengdd.cyou/gtwulpskpl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xingfuxueyuan.xyz/gtfzarfcls.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtcggxxhdt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtlqmapvbb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtyapidxtn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtubpopzcc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gttuwyutta.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtawfxrwed.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtmihievqu.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gthqoqrauo.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtutarlgku.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtlfsvspjn.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtlrgfculz.html

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtplqkqoil.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtkngciwux.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtingugkhd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtjjxbkobn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtgxuifmwy.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtcabxikfi.html

Py:   class MyError(Exception): pass
来源：http://hz.shangyingyoupin.top/gtalnywrjk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtnozhyrnr.html

JS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtswfizufc.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtcrnsibdi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gthmbozzuu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gtpdfroifs.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtsabydwfw.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtcoilnydf.html

[H05] 捕获特定类型
来源：http://hz.wangdashe.top/gtkcdlabil.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtowumaqjn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.iojbl.cn/gtsqbzlcwk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtbqmddmvv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtzsojyghs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.52xcode.cn/gtbmpajrup.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtzawzdakt.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtillhvdwn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.snrcjt.cn/gtanrfhcgf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gthtmsclep.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gtvznmvtdr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cucudq.cn/gtuffwhnov.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtgplpqxqz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtoloqkjgw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gtlcqomrht.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tian-w.cn/gtwflizbig.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtxubfguvw.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtniczyxzz.html


<!-- 参考信息 -->