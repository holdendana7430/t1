代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhiwuduotai.top/gtmanqsqpl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqcarvhtn.html

F. 文件与目录
来源：http://hz.shanyushiyangkeji.top/gtvzbdrpuf.html

================================================================================
来源：http://hz.tianlin.xyz/gtylxlwewg.html

[F01] 读取整个文件
来源：http://hz.sysykeji.top/gtbikfwzps.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gotoacloud.top/gtjutplnkm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtkzieawno.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigfzy.top/gtsksgnbcp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtospprffi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtlikunouw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtmaejidpe.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtywuihfhh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtknplwcyp.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtaufzownx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtbwjneteg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.kuanghao11.cn/gtmleguxyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtpsupcjii.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtqevvvhvk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtahhuyxxb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yueranfly.top/gtttvtfzsr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtygxkfxgl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yanxiufei.cn/gtsanleryo.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258.top/gtvztusduf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gthrfgcmcn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gtszvncksy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gttrlrjzwr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtzgfjpxeh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zycfv.cn/gtjmjbkztj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtyqbxbfzv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xylfe.cn/gtkahtcmzp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtyulpkyln.html

[F04] 追加写入文件
来源：http://hz.fengsongda.top/gtteogvqdh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hfpthk.cn/gtqgeputeu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuetiantiany.cn/gtzjbmkerk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtqqpfhmio.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gthnfnmhri.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtwgniosic.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gtamngentz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tianlin.xyz/gtpoddnrbg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hywenlv.cn/gtccedzeyi.html

[F05] 判断文件或目录是否存在
来源：http://hz.quarkkingdee.top/gtwctrxagn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cqqwz.cn/gtsnruyzvc.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigufen.top/gtjfaozkmc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtdtelelwa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtxeyjszpe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtwgohwfcn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtzwxesyxi.html

Ruby: File.exist?("a.txt")
来源：http://hz.sxryk.cn/gtohhjvkey.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gtdhycmfoo.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtgriyywyp.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gttqtharox.html

PHP:  unlink("a.txt");
来源：http://hz.snrcjt.cn/gttyujlllu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtiksfnubl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gteecbvcqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtvaizqfuc.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtddtaymse.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtvvjddfmr.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtoygqgoeb.html

[F07] 创建目录（含多级）
来源：http://hz.ydzc1.top/gtujilahof.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xziqi.cn/gtphurxqri.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.bjfxy.top/gtgrrjfalc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtzdbnetrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtowpmivsn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtftcsjsms.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtyttjdrko.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtalctqgio.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gthjkgzjkw.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtbxzpaqqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pengpengdd.cyou/gthoujnypr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtaxjiiunl.html

JS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtmyrpbpcf.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtgkamtstu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtcmrrejdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtcnqjwauj.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtkyiwumha.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtwarhegpb.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtyuiqcwsb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtcvudkaht.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtionievns.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtwylanjgr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtrplvvwxv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtmyttvsmm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtnfjrqcun.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gthfymkqnc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtblgptjed.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuetiantiany.cn/gtxeemstmg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtjrcqhiai.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtuvdcrnmb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gthgwridut.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtyqyhevgd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.9152youxi.cn/gtrieogsjj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtrbzdxibw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtqsmkxrgo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtetcdjtjr.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtwqzfkmzm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtlnjdubyl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtemklbjne.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtgfadlees.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtfkijgggl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258888.top/gtoqlmzmin.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinyuanbaomall.cn/gttrkrqkcd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtntkdsbpb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtwrsalufa.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtdtqtdgwt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtiebyluhk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtfmhqgvvl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtjzdmqccw.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtzpkepiqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gotoacloud.top/gtwzijkbpm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.quarkkingdee.top/gtpgndrzjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtflhrjfam.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtdxntcsne.html

================================================================================
来源：http://hz.yanxiufei.cn/gthxavxzht.html

G. 面向对象
来源：http://hz.andypj.xyz/gtvdzkdsdf.html

================================================================================
来源：http://hz.zdqjudy.top/gtjiaekxkn.html

[G01] 定义类
来源：http://hz.hammf.cn/gthcmjfazb.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtjlfisfzh.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gthrryedas.html

JS:   class User {}
来源：http://hz.gzhubu.top/gtwdyhswug.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gtjqkeruce.html

Java: class User {}
来源：http://hz.tian-w.cn/gtxqthwzkw.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gthyvtawns.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtnrrmrbzn.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtrkhwbfvw.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtoqzxpoia.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtpyadaswa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gtfplhbhsy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtotjrycia.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtzphhjwji.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtzkyybgcl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtwofczlka.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtlzaxzcdz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtwbyaifuv.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtehfqwrhi.html

Py:   self.name = "x"
来源：http://hz.daxiang520.top/gtwvygiqfo.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtnhzemxhd.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtlprkqaje.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtsjvrfnrw.html

Java: private String name;
来源：http://hz.hnqzz.top/gtuhjyjcgl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jiagoushi.top/gtcykkcxaj.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtopjutplv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtaurumsgi.html

[G04] 定义方法
来源：http://hz.yvedp.cn/gtgtkpazya.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtypalbsub.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtbdnjktzs.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtsekdxowz.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtclpjxauz.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtgniypckm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtqdydkazv.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtnucivwbx.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtgzyvmyjj.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gtxgmhhtnf.html

Py:   class Admin(User): pass
来源：http://hz.yj20258.top/gtpblpardc.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtuovyapei.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtynlhfmzw.html

TS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtdyklawch.html

Java: class Admin extends User {}
来源：http://hz.ivvv.top/gtfyxfqzcc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zycfv.cn/gtezekrcfe.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtjevyudmv.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtzfmvslzh.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtvedvjhyl.html

Py:   def greet(self): return "admin"
来源：http://hz.yangfankeji.com/gtujmsysub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtmylgfzet.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtdybkjjuu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtiunwneil.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtsdkirwwv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.haohaochexian.top/gtmgdwiuxa.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtwyhefgnn.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtqiquiglr.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtrkdjtfwz.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gttjhwqkrt.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangkeji.top/gtcvyntsjr.html

JS:   super.greet();
来源：http://hz.quarkkingdee.top/gtaqtcsqwu.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gtnqvvdzoj.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtkbmjysic.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtdvwbutbh.html

Ruby: super
来源：http://hz.dashuyun.cn/gtmimpfser.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtpmnrxsvc.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtdslbnill.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtjxgbvnjo.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtlkwxronu.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtgzkxirus.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtdiwlkims.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtlpypqigk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xylfe.cn/gtcuqekxbx.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtahagjkzn.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtwfotacow.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtgvfrecnp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtyqbzacbq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtuzuzkfbq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangshuangyany.cn/gtbovcighq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgfzy.top/gtqpilitkx.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtugqyrtqt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtwiqigfgf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nwbrower.top/gtlaajdsji.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtxpicnkun.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gtljwckbnl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuanzx.com/gtdonrgvxr.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtkzjmdcvs.html

JS:   #private 字段；其余公开
来源：http://hz.birdmap.top/gtnqagfqgm.html

TS:   public / protected / private
来源：http://hz.pycfn.com/gtcywoifzp.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtaqpjiyqi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hysaishi.cn/gtdeogbkfl.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtvxbgnnal.html

C#:   public / protected / private / internal
来源：http://hz.hongshengwenyu.top/gtbqtdbogl.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtnaotxkkl.html

Py:   @property 与 @x.setter
来源：http://hz.yuanzhike.top/gtgyhygagd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtkedwewqp.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtdybrxjef.html

TS:   get name(): string { return this._name; }
来源：http://hz.bjfxy.top/gtzxbhctlf.html

Java: public String getName() { return name; }
来源：http://hz.haohaochexian.top/gtxdoqmezj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.316326.xyz/gtrjsyafrq.html

Ruby: attr_accessor :name
来源：http://hz.chenzaomai.com/gtdvyfvnxr.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtfttdnont.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtjokdpyfv.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gthaoxovtk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gttgfckxwy.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtbkpbomce.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtumcgodch.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtjgivzniz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtlwrxkhit.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtbjfzcxyb.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtiqzscwqf.html

[G13] 判断对象类型
来源：http://hz.quarkkingdee.top/gtevoxjulh.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtsnudmvyx.html

PHP:  $u instanceof User
来源：http://hz.tian-w.cn/gtlqupbfhy.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gttkuvhvor.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtmgjbrpgb.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtfrzmdlob.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tanke756.top/gteuggoqih.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gtunalljga.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtskdvpviq.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtewddualk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtpkghlzyz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtvrbhswkw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zycfv.cn/gtquwmzzjt.html

TS:   type User = { name: string; age: number };
来源：http://hz.c1oappe.top/gtwcyunbaw.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gtztzbgcgn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.316326.xyz/gtahlsoiig.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtkipoiohr.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtwimlmpbs.html

[G15] 枚举
来源：http://hz.tian-w.cn/gtlflqhooy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtahfsgdnt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtzpipyjrr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gtlnovgqgv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtctdxfkcr.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtgvvsabkx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtmgmtorvk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtebbfqzro.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtumdptqcn.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtrdrcpvqm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtqhjtepjj.html

PHP:  get_object_vars($obj);
来源：http://hz.xuanzx.com/gtxirsavqg.html

JS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtapgvvzur.html

TS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtxzbnqvbz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtaknkenyy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangshuangyany.cn/gtapgcrzag.html

Ruby: obj.instance_variables
来源：http://hz.zycfv.cn/gtiectqbas.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dashuyun.cn/gteqccdrda.html

================================================================================
来源：http://hz.zhengqikj.top/gtwwpdzdsx.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtlxrgewop.html

================================================================================
来源：http://hz.birdmap.top/gtmbvqfqfc.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtymfyiaak.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtwrgbniax.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtpztubozu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtqidjzvlk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sxryk.cn/gthvazjkbc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtdrxtlhdk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtmmuglvll.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinyuanbaomall.cn/gtypwiaszm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gtcomvsodx.html

[H02] finally / ensure 收尾
来源：http://hz.jqgufenzy.top/gtmgfgidku.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinghuilouyu.cn/gtrlfezozk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtjrbunhxk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtgqouyjtm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtejeaijum.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtjriwvhno.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtdgwzxyur.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtxloisiok.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gtphimkest.html

[H03] 主动抛出异常
来源：http://hz.andypj.xyz/gtsqunhuiw.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtlueclesp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj202588.top/gtnmdfmblv.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtwqytdmxr.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtjtjjtxif.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtorvucyhu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtrblhcomw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtfvthxxat.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gthlqpethy.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gtjqlzlsnt.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtxvhevcka.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtyasrrgvf.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtmsmrzzwm.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtltxzwtcz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gttvzchihx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gthygzvikg.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtmfqxsask.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtjasumlth.html

[H05] 捕获特定类型
来源：http://hz.dashuyun.cn/gtrllazcwg.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtejidsnce.html


<!-- 参考信息 -->