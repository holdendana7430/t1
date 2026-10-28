代发 wailian999

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtcasjnmfp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gthsvjetyn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jiagoushi.top/gtekehowtv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnxiangtu.top/gtzwblelof.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtowcianac.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtufphwvjs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtlftckxsb.html

Ruby: File.read("a.txt")
来源：http://hz.yongpay.top/gtlidyjucs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gthrraxbnj.html

[F02] 逐行读取文件
来源：http://hz.meibo888.top/gtwvlqdzqq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhengqikj.top/gtsfdevxup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtahrolwzj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtiuewsnlp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gttcjjejbd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtobxakojv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuetiantiany.cn/gtqswmwhjv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtgfgqvblj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigfzy.top/gtdpbpsuor.html

[F03] 写入文件（覆盖）
来源：http://hz.mhx1999.top/gtanbecrln.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtumstrscz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tianlin.xyz/gtsritqjiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gttzomiize.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtowxpqeeb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtkizmelks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnxiangtu.top/gtjrxpasmh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zycfv.cn/gtloilcyxk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gtjkmalkyp.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangkeji.top/gtbfkcfpbj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.havefunace.top/gtmgmplfta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtjpgxyove.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtztdlwlkb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtyckmsvng.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtojqbprmq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtjblhvhdx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenlongwang.top/gtufqcresv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtcytuhtpj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtargipnof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gturcytkbf.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtabtctmsc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtofhvxnzg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtorrtagdi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtviynuepv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtqxxbynjb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtxujhyaya.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtaigikbkw.html

[F06] 删除文件
来源：http://hz.ybcxt.top/gtdsussszq.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gteybwvgeo.html

PHP:  unlink("a.txt");
来源：http://hz.zdqjudy.top/gtvgechvrx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtkmmblycb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtblvhynjd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtmmtrozdb.html

Go:   os.Remove("a.txt")
来源：http://hz.aibaodan.cn/gtxdcsuqrg.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtgonsyxlq.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgufenzy.top/gtejexrtvm.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtvwurwxie.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gtswqrhokq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtqkkcahme.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtgidkgczl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtcnfsedqm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtwdygqmml.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtrilqhenk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.feifeiyinyue.top/gtwxezhffi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aizwys.cn/gtguozbqje.html

[F08] 遍历目录
来源：http://hz.zdqjudy.top/gtpgwpjsxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgufenzy.top/gtxgzkqint.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtcyzddbhe.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtowdkaahi.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtixcctoro.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtosxitlkf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtvpyxemrc.html

Ruby: Dir.children("dir")
来源：http://hz.sysykeji.top/gtygdyjhhu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtptvqrmlj.html

[F09] 获取文件大小
来源：http://hz.daria6918.cn/gtanygifud.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yongpay.top/gtzfxjjpvl.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtkbghagqz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gttjjvnkuu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtojaiaayw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtogdivsrx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gtlzzilslq.html

Ruby: File.size("a.txt")
来源：http://hz.bjfxy.top/gtrnrnpadf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtanksenye.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gtyrbufolo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtskcsuuuw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ppjwa.cn/gtjdnkyyhm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtymaxytsy.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtczdgrwnw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhixingplan.top/gteumxncbc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gotoacloud.top/gttrgackqi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtroogmbip.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtajihlxuc.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtwtscynom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtxmbdzwiv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ppjwa.cn/gtpcbhsocn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtepxuijij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtlpvutmir.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.mhx1999.top/gtdukcqqxd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daxiang520.top/gtvlmgzrmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtyxyucpqs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtrcixyxyd.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtvqbbfhyl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtomwbbbue.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtfzzhglff.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtkzfghvim.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtrcphffny.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gzhubu.top/gtrfhzcyvp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtxanhtjhx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtdnkkragy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtemokxcco.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtapwgxipc.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtxkhnhlkc.html

================================================================================
来源：http://hz.tian-w.cn/gtqltysvnv.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtcxsmcrgf.html

Py:   class User: pass
来源：http://hz.pengpengdd.cyou/gtjhdocfix.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gthfsjbmhm.html

JS:   class User {}
来源：http://hz.fzhhl.top/gttzbsrnei.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtjdeourpt.html

Java: class User {}
来源：http://hz.nwbrower.top/gtizhhklbp.html

Go:   type User struct { Name string }
来源：http://hz.havefunace.top/gtvmqzawih.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtfvgptcdf.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtfkbgawcc.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtgtqvofdc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtcdqduhsz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtabayqdig.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daria6918.cn/gtdtlygobt.html

TS:   constructor(public name: string) {}
来源：http://hz.aizwys.cn/gtjqykrpzv.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtfzheaeno.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtzpclbojx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtusgcbths.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtljhkrznn.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtdnvdsdkp.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtqieophhm.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtodtwalgz.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gttkwltjeu.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtihubqzet.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtgnmentwf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtqrsefsam.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtagrlsdjy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gaohongyu789.top/gtuwspjfgm.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gtcxxvkdzf.html

Py:   def greet(self): return self.name
来源：http://hz.fzhhl.top/gtaltlucvd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtplqzhcmr.html

JS:   greet() { return this.name; }
来源：http://hz.0kj1m.cn/gtmnqnigts.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtfqafefyd.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gthdpwwwsw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtbuubhelu.html

Ruby: def greet; @name; end
来源：http://hz.yongpay.top/gthqazraij.html

C#:   public string Greet() => Name;
来源：http://hz.aibaodan.cn/gtxbfmqcnh.html

[G05] 继承
来源：http://hz.yanxiufei.cn/gtizhpwond.html

Py:   class Admin(User): pass
来源：http://hz.hywenlv.cn/gtsorweued.html

PHP:  class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gthuawqczb.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtekepxoih.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtjfpzrkzl.html

Java: class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtlwezwjqd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigufen.top/gtsxojelss.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gtowwqqozf.html

C#:   class Admin : User {}
来源：http://hz.iojbl.cn/gtawxjctku.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtultymlmw.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtusdatvgn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtnynanfra.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtpomywpeb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtqvkrkwuv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtcwugrdqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtjfovzudj.html

Ruby: def greet; "admin"; end
来源：http://hz.meibo888.top/gtyjattogq.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenzaomai.com/gtqqqbgsnc.html

[G07] 调用父类方法
来源：http://hz.yangfankeji.com/gthkxqeljw.html

Py:   super().greet()
来源：http://hz.316326.xyz/gtwmxxscfy.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtgwngqauk.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtwkjctmlm.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtstaeydsm.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtiizkmhle.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gtjbpdorfs.html

Ruby: super
来源：http://hz.hfpthk.cn/gttihfyuge.html

C#:   base.Greet();
来源：http://hz.tanke756.top/gtkyxrvnmg.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtkwjtrymi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtsyhocmmb.html

PHP:  public static function f() {}
来源：http://hz.hnxiangtu.top/gtdawnzmpp.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtaybzmrqu.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gticxwzhpu.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtntckubiv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtsjfrbhdh.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtohavwoik.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtksdghkrd.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtzihvfwgn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtbqnnnuuq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.52xcode.cn/gtxusoocxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtnrblatgg.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gtxawdidgg.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtxzidhedb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gtvcmwvxib.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258.top/gtooxpibbc.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnxiangtu.top/gtwqoabeoi.html

[G10] 访问控制
来源：http://hz.cdnleiting.top/gtdleutmsq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtqdcnyrkv.html

PHP:  public / protected / private
来源：http://hz.ydzc1.top/gtxvrpxpqd.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtjthlwtib.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtwvuoodfy.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtptzalobx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj202588.top/gthgphjuzr.html

Ruby: public / protected / private
来源：http://hz.smart0.xyz/gtqhnwyemi.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gtetumzxtk.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gtxmxluosl.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtqwhdgawu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtydkfwubp.html

JS:   get name() { return this._name; }
来源：http://hz.wangshuangyany.cn/gtepfygrne.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtuddiutqe.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtwmswnbjt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtejrxacvj.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtpsmhjqjg.html

C#:   public string Name { get; set; }
来源：http://hz.hywenlv.cn/gtiaurhihg.html

[G12] 对象转字符串
来源：http://hz.c1oappe.top/gtnpzbcpag.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gtbhrhfbqj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gttnbwbqaw.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtznqcmnym.html

TS:   toString(): string { return this.name; }
来源：http://hz.xinyue.icu/gtjsjgwczn.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtyfiijzis.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtkwajslwg.html

Ruby: def to_s; @name; end
来源：http://hz.gzhubu.top/gtdlzxpbpn.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtheqlpeqn.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtfakrybix.html

Py:   isinstance(u, User)
来源：http://hz.ppjwa.cn/gtfihkrejz.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gterpozdfn.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtqfczigjv.html

TS:   u instanceof User
来源：http://hz.jyoumei.cn/gtnjbafful.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtoglisrvb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gticwmrcrf.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtfepdmwdz.html

C#:   u is User
来源：http://hz.pycfn.com/gtqicqxesd.html

[G14] 数据类 / record
来源：http://hz.cqqwz.cn/gtysvovmbb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gthoglqaze.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gteailzzra.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gtkhshcxwt.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtsgsufvcx.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gtlvdqlppd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtpamhxqrv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtfmroyaii.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gtpymfvmhs.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtvquzloxi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinyuanbaomall.cn/gtzwelvzhh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtffninnhb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtumgwnavs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtvsxooydq.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtfrwgmwnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuanzx.com/gtaycekmrh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhongyouzk.top/gtmnmjoacj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gturhatdjv.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gtymwlfxio.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtkjraqdxc.html

PHP:  get_object_vars($obj);
来源：http://hz.gzhubu.top/gtgbmxwagv.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtpswhtqfg.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtzktputbr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtevpmgvuo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtyhojgsqj.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtamlybfxf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtwsfduniw.html

================================================================================
来源：http://hz.yueranfly.top/gtqqeywoxk.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtqbrwzlni.html

================================================================================
来源：http://hz.dashuyun.cn/gtiznzebiu.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtojhuenho.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtuficubdk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtxfuvrkmt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtlucvsbcx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guannengcc.top/gtzsamndmi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtujqhntoq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gttfrxmnvf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtpubwbuuy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gtzvxioxug.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtzseawnsx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sufxvd.cn/gtyfgbnhru.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtykleawza.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtmbtxvcrl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtoxqpfgnd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtddohrgcz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtovmfypyt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtugzaylqu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.birdmap.top/gtfcvlcibd.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtcpefjzqz.html

Py:   raise ValueError("错误信息")
来源：http://hz.9152youxi.cn/gthrwragsz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtgkbsobqd.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtolttttyw.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtqrbrthzz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtitfmjoui.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtehzahgmy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gtnunyqchn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtcgorlsqv.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtuicfgepo.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtnynovchi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.svipenyu.cn/gttvfddxqm.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtstcjnyln.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtwurruzqf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtupxwirnu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtcifttnux.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtuwtiyalg.html

C#:   class MyException : Exception {}
来源：http://hz.quarkkingdee.top/gtwjzzpybr.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtjbxkanfq.html

Py:   except ValueError as e:
来源：http://hz.jinqigufen.top/gtzjwrtjlp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtmvmdmzhd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtzvbiynar.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtyhxlywan.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gtozbyjsck.html


<!-- 参考信息 -->