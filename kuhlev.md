代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtytizocui.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tianlin.xyz/gtatsasviv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtswoxlysc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtbnfumbdr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtbysjlftv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gtjqzwdbtv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtbhlfzdhy.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtxhjhwrap.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxinkj.top/gtimmuowfl.html

================================================================================
来源：http://hz.yangfankeji.com/gtdqmddlqd.html

F. 文件与目录
来源：http://hz.guowangkeji.top/gtvdovxbcr.html

================================================================================
来源：http://hz.daxiang520.top/gtxhpfrlqj.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtdkjomwyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtcfoqtzhd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtgynaxmbz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258888.top/gthctdqdmc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtfdpxjbqr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtvxayahtc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yonumen.top/gtbjayucdr.html

Ruby: File.read("a.txt")
来源：http://hz.nwbrower.top/gtcxchmrwu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtwadedtck.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtgnwazelm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtoqjgegmz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgufenzy.top/gthcvoqnxl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtdrhbitix.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtswtspsbh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtfdbmfasz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtknkbdxoh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtbaugrmbv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtdoupeonc.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtywzizjkn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtmrumdevi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtdpngfean.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gthyhgzaex.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtlljlbuoa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtgyikhpyd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtgbbcdrwl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daria6918.cn/gtudxnzedo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtfamutsoa.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtgduobetk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gtrnjkxxqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtcfxsvdkw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtcaqoctzh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtgdqqtwac.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shangyingyoupin.top/gtmtpojjia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtbtkivcti.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtmsflnkmu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtvejkqeig.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gtwzrqfxnr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtpygkqyxr.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtdeljbdrg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtjjzhltya.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtwladfigy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtyguiklsh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jlsjyb.cn/gtcmoqszdr.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtdaucqevk.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtjyzdftyr.html

[F06] 删除文件
来源：http://hz.dianchejie.cn/gtpafdftrv.html

Py:   os.remove("a.txt")
来源：http://hz.hnxiangtu.top/gtwpsbajmz.html

PHP:  unlink("a.txt");
来源：http://hz.ydzc1.top/gtkuyaaeqf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtstavgwht.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtgahdgajv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtjuavmahi.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gtqdueozgp.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtndhcgktr.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gtwdewjrih.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtmznzvzpj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhongyouzk.top/gttfbebuvu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtrlnuytzy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtdudtqdjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtuvktwsww.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtwttbxglc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.0kj1m.cn/gtwicftfbh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtkoqgvhsy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yonumen.top/gtjkgyjwyh.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtvkdawqvo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtsyyglnkb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtahiyvksw.html

JS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtmjtsryoy.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtnpiaaoxt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtcjurgzzp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtfmtiwsws.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtengivtuy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gttopobawp.html

[F09] 获取文件大小
来源：http://hz.chenzaomai.com/gtorwtcjyh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtzsrmilwy.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtkzjiqkon.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtnouzfzlk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtkihgcxvo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtxaegocnz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cucudq.cn/gtyxhyxvmj.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtgtedksby.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.haohaochexian.top/gtstmcympz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtqoexpgvc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtlgsypoyg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.bjfxy.top/gtcpwgtmqr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtkbvudhng.html

TS:   path.extname("a.txt")
来源：http://hz.wangdashe.top/gtujaueqpq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtziqjnbmx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtytvtaole.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtuyytxrru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtofbqrlwr.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gthelnjjsg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtqgpzrkwv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.iojbl.cn/gtlyoxwcrr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtxdaxxtnv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtsuhkhwhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangkeji.top/gttqpngsbr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.haohaochexian.top/gtjbxbnwjp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtuzkjsgeu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shuidangran.top/gtgwyepzvm.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gttwygcpuu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gthgwqdikp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtmwjflzrb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtkulqklhk.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtmhhzmgbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.c1oappe.top/gtlvisiicg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtthrozsey.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gthpuodwbm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guannengcc.top/gtitfysqjl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkgejlwoj.html

G. 面向对象
来源：http://hz.xuanzx.com/gtbzfnfdnf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtvssfcdpf.html

[G01] 定义类
来源：http://hz.hysaishi.cn/gtwlydtnwg.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtplrucbyw.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtkshsiwjz.html

JS:   class User {}
来源：http://hz.jinqigufen.top/gtdhkzdarj.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtlfbccevb.html

Java: class User {}
来源：http://hz.quarkkingdee.top/gtqloexaqq.html

Go:   type User struct { Name string }
来源：http://hz.mhx1999.top/gtegrgoduj.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtpxcexdun.html

C#:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtxxbatlbx.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtjvtrxrth.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ppjwa.cn/gtmpbrgpfb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtdkxfyxnx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtzylznfte.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gteakvpulr.html

Java: User(String name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtivobmduk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtcgggyaqt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtauqnbfxh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtawyvdkmt.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtngmwuruu.html

Py:   self.name = "x"
来源：http://hz.zycfv.cn/gtnejthyax.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtzxfldbdt.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtjyogdhgr.html

TS:   name: string = "x";
来源：http://hz.yuanzhike.top/gtqsqjctii.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtmyhcrnjs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zdqjudy.top/gtumbucivs.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gtateavnbs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtyecrddhm.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtkzqnufmv.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gthlawrwdt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gthiiheqzt.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtzgedmkwf.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtqzsofeum.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtrfwmdxax.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtcyaxrhqg.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtspvhgwhn.html

C#:   public string Greet() => Name;
来源：http://hz.ydzc1.top/gtnkpezaqo.html

[G05] 继承
来源：http://hz.sysykeji.top/gtyatolnmr.html

Py:   class Admin(User): pass
来源：http://hz.kuanghao11.cn/gtflacxmal.html

PHP:  class Admin extends User {}
来源：http://hz.pycfn.com/gtkwftpgql.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtpwkezwxu.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtnthhsnss.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtwipbypid.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.meibo888.top/gtxyiymtzs.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtxbnuatpr.html

C#:   class Admin : User {}
来源：http://hz.svipenyu.cn/gtnqhkwglb.html

[G06] 重写方法
来源：http://hz.cheryme.top/gtvhoghbxw.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtixfqwxdm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtdpirzdhq.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtkcyvsdlr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtypnwmyzh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtgittjkrn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtylozjuyi.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtgshojutl.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhongyouzk.top/gtvqjqkves.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtzhoipwpy.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtgcpmfgwo.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtenrmqfre.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gthfitfqid.html

TS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtnawfyoxd.html

Java: super.greet();
来源：http://hz.316326.xyz/gtuabqeobt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ppjwa.cn/gtgszyfufp.html

Ruby: super
来源：http://hz.dianchejie.cn/gtrazzqoks.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtbeivwexo.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gtawmigxrj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtgqglrddz.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gtabcdpeyq.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gttvvnlykr.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gtqlthjmcf.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtcifgzrco.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtbcavdkyh.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtzafxpogo.html

C#:   public static void F() {}
来源：http://hz.xziqi.cn/gtxvasabks.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtxdrmndyg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtzseyiksf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gthjfmeeho.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtdqoyitvo.html

TS:   interface Shape { area(): number; }
来源：http://hz.sxryk.cn/gtjulcyhzl.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtmevhjsyj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtlykaukbq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtjprjxxft.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtvtomxbiu.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gtcshwsfog.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtyfecqodi.html

PHP:  public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtgvevxtsq.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtofpvnlei.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtemhpatuz.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gttqynairw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtecagcqpg.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtjavmmmbc.html

C#:   public / protected / private / internal
来源：http://hz.fzhhl.top/gtiphfhvzw.html

[G11] getter / setter
来源：http://hz.c1oappe.top/gtchqgvftp.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtfolyjmdm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtvneezfvl.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtauylwgib.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtudtleyzh.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtqmgorywu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gtatwhahsn.html

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gtdvqaoria.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtafksbltq.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtyxfmktwp.html

Py:   def __str__(self): return self.name
来源：http://hz.yongpay.top/gttluomjuh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtcvdxnbwl.html

JS:   toString() { return this.name; }
来源：http://hz.andypj.xyz/gteorjjqym.html

TS:   toString(): string { return this.name; }
来源：http://hz.shuidangran.top/gtocahguzq.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnqzz.top/gtllvebnvv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daria6918.cn/gtyvjelhqy.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gttjoazzfm.html

C#:   public override string ToString() => Name;
来源：http://hz.zhijiandao.cn/gtaeazucqs.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtjzywvrqg.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtqnsnlnio.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gthcfndrhd.html

JS:   u instanceof User
来源：http://hz.hywenlv.cn/gtjlnyyvzl.html

TS:   u instanceof User
来源：http://hz.snrcjt.cn/gtnjwfwehw.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtqflxbtuj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xingfuxueyuan.xyz/gtkbibufpc.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gtawucbfbf.html

C#:   u is User
来源：http://hz.smart0.xyz/gtdnfqkjwb.html

[G14] 数据类 / record
来源：http://hz.yuxming.cn/gtskjekltx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtrfoedrmp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuetiantiany.cn/gteyutlasl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aibaodan.cn/gtfcvggpsx.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gttmfhmzmf.html

Java: record User(String name, int age) {}
来源：http://hz.snrcjt.cn/gtmbgkzwdc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.quarkkingdee.top/gtvpgkazph.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hywenlv.cn/gtqfzdevsp.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtatytrqqz.html

[G15] 枚举
来源：http://hz.yj202588.top/gtxrspfbuo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtdincycek.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtkkkpaysj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtikajjfuf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtjwgaovhm.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtwqtjsiyh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtddmjhmrl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jiagoushi.top/gthwpcfilm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtpiiwiwdk.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gtyxkqonqz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtnntdzwuj.html

PHP:  get_object_vars($obj);
来源：http://hz.ppjwa.cn/gthipfhhcw.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtjpoajjot.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gttkaxclqs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gotoacloud.top/gtvnaamtrn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtgrxuerdy.html

Ruby: obj.instance_variables
来源：http://hz.jinghuilouyu.cn/gtuzrctyyk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnxiangtu.top/gtqwktujtn.html

================================================================================
来源：http://hz.sxryk.cn/gtqsvsqkhp.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtfkwfxmry.html

================================================================================
来源：http://hz.ehwqpu.com/gtmiwdfnux.html

[H01] try / catch 基础
来源：http://hz.hnqzz.top/gttyijebaj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtotgifhxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtucghdtpj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtplxnqnrx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xziqi.cn/gtrhtxlifw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xingfuxueyuan.xyz/gtxskinsit.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gturzxwrlu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtbgustgow.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtayrgedok.html

[H02] finally / ensure 收尾
来源：http://hz.tanke756.top/gtqjhatfqt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cashguo.top/gttwpekjhj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtbyunlvuv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtpdzkcpmo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtbyukleel.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gticcdjsdb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gttkletdyl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sxryk.cn/gtwnadhvdz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dashuyun.cn/gtchbisvjl.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gttdvjmobd.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtyhhazcyq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtopnjmsbu.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtdyzrtnnb.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtvuchxuru.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtvzbszibs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtgumthxcv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dashuyun.cn/gtwxuqoazp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xinyue.icu/gthptqdpji.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gtdecrbquz.html

Py:   class MyError(Exception): pass
来源：http://hz.fengsongda.top/gtztwtvgph.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtzoogravs.html


<!-- 参考信息 -->