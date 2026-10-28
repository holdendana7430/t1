代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtduhqqryo.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjbfjiqcb.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtcjqjvbjh.html

================================================================================
来源：http://hz.guowangkeji.top/gtmvkgwuzs.html

[F01] 读取整个文件
来源：http://hz.jianghu66.top/gtuoqncgks.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtyxvwvflg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gttgrfpuzc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xuetiantiany.cn/gtytqahzby.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258888.top/gtocetvzji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtzrzohfit.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangshuangyany.cn/gteotqghiu.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtazhwfruf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dianchejie.cn/gtmbidfzeq.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtggqkwqgv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtmqxeencw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daxiang520.top/gtagtdykxn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtarlmcyck.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gthgipzvic.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtckybfhks.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sweek.top/gtsigwtdsk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gtkthjrqyh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gtpvqithnj.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gtbojlcghc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtsisqedny.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtbjreholq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gttgnzyfxy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtnbxhgudl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtdckxoncs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtlyrohetn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtstqynaub.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtpbifoqgt.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gtwhnqpsfz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtsgkgizzw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtcyrmikqp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtxupitfmo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtecpgpzgx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xingfuxueyuan.xyz/gtpoipegyc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtodzplwfo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shzxlz.cn/gtwrcecdxi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258888.top/gtkutytvni.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigufen.top/gtjhzlnwau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hammf.cn/gtmsrjstfe.html

PHP:  file_exists("a.txt");
来源：http://hz.ydzc1.top/gtenmstxke.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtdibxncjj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtidrputth.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtupszygfm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gtmbzyzvxr.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtuzhqubzj.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtnhcyeecm.html

[F06] 删除文件
来源：http://hz.zhijiandao.cn/gtucwfbbcn.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtvcirhxsj.html

PHP:  unlink("a.txt");
来源：http://hz.shuidangran.top/gtsaapeevw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtbkwerpel.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtutjguerz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtikmbrqqv.html

Go:   os.Remove("a.txt")
来源：http://hz.ybcxt.top/gtzpshclrs.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtsgbizfml.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtzrryxhyb.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gtqtfynjnq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.smart0.xyz/gtbtjnqrix.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhaomingkeji.xyz/gthgmddjum.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtzzvvdvoa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtorxztwjo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gtwyfdwlqd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtaszhetgt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtvckagfer.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydzc1.top/gtrfmxzwum.html

[F08] 遍历目录
来源：http://hz.yueranfly.top/gtlhtrzhca.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pengpengdd.cyou/gtslpxfwnz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gttwiobtzl.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtznvibhyx.html

TS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtmgtfteiw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtvinpkrfe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenjidiqi.icu/gtgtglyzcc.html

Ruby: Dir.children("dir")
来源：http://hz.smart0.xyz/gteugfwczf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.c1oappe.top/gtheyblquh.html

[F09] 获取文件大小
来源：http://hz.dashuyun.cn/gtneongcby.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtiyolhqys.html

PHP:  filesize("a.txt");
来源：http://hz.zdqjudy.top/gtwbffxzbn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtvqqbhjna.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtvsnbmsvi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gttdzyuyjf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zdqjudy.top/gttocyyqxc.html

Ruby: File.size("a.txt")
来源：http://hz.sufxvd.cn/gtpauqceku.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.9152youxi.cn/gtwmzoiamf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtjjtvpkho.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtphxrcopf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.iojbl.cn/gtbpabdtmq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtcdxwbjne.html

TS:   path.extname("a.txt")
来源：http://hz.sxryk.cn/gtmatzjhwm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.iojbl.cn/gtpftwknuz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtbgvwjkdv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtjtbhnjqp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtputcctrv.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gtwjlszuxe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtlkhhnnxk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zycfv.cn/gtebimrwqb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtdsdixqmi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gteybsfnpd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtsnilpfce.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtstxyyczd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtaawskyom.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtenetmgrl.html

[F12] CSV 读写
来源：http://hz.yuxming.cn/gtpmxnypfm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aibaodan.cn/gtfhxcjzdz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtngiofibh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtxhrdkucs.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtbrmuupjp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fengsongda.top/gtazriqquu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gttxvfskwr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtrflspbjb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtfbfykjtl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjshvdmul.html

G. 面向对象
来源：http://hz.mhx1999.top/gtfptcmtoe.html

================================================================================
来源：http://hz.chenzaomai.com/gtvgewlxit.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtuarqgpgq.html

Py:   class User: pass
来源：http://hz.daria6918.cn/gtadurhndt.html

PHP:  class User {}
来源：http://hz.fengsongda.top/gthitxshln.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtkagoaaxu.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtgezhtjyy.html

Java: class User {}
来源：http://hz.dianchejie.cn/gtydvaovaq.html

Go:   type User struct { Name string }
来源：http://hz.mhx1999.top/gtvvnwvbti.html

Ruby: class User; end
来源：http://hz.yuanzhike.top/gtgglcnwbz.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtrqrtmytf.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtagpisbaz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtevvwglok.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gttemugomh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtqgrrzrvr.html

TS:   constructor(public name: string) {}
来源：http://hz.bjfxy.top/gtkrduuywz.html

Java: User(String name) { this.name = name; }
来源：http://hz.yvedp.cn/gtlhvtttzd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtxacuxdry.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hfpthk.cn/gthonujbao.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gttptmtjpm.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtltmkihht.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtpnestsww.html

PHP:  public string $name = "x";
来源：http://hz.feifeiyinyue.top/gtuufzhjma.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtdlatgrix.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gttvpupzkc.html

Java: private String name;
来源：http://hz.bjfxy.top/gtmdqoescs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydjk.org.cn/gtuvgiqczv.html

Ruby: @name = "x"
来源：http://hz.kuanghao11.cn/gtgynewnjb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gzhubu.top/gtaevmdqqo.html

[G04] 定义方法
来源：http://hz.sweek.top/gtjerhmqzk.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gthevtgerz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtuwscjhpl.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtrajeewjr.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtxcymepmn.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gteeefycgk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtxofgniqu.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtovdtfhij.html

C#:   public string Greet() => Name;
来源：http://hz.xylfe.cn/gtunpxaobg.html

[G05] 继承
来源：http://hz.shanyushiyangkeji.top/gtyogbtnfx.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtlbltqkcq.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtblkivvsn.html

JS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtlyzsdiso.html

TS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtlqkgzdko.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtfoqpjzpd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtxvhaycgg.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtqdclpqur.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtnpcrvvke.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtgnixtgpb.html

Py:   def greet(self): return "admin"
来源：http://hz.hfpthk.cn/gtjexunxmh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtomfmlfjk.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtpphhjygq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtbmqersbs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtjsycjbrw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pycfn.com/gtjcwdfpek.html

Ruby: def greet; "admin"; end
来源：http://hz.guannengcc.top/gtheyfhbbw.html

C#:   public override string Greet() => "admin";
来源：http://hz.svipenyu.cn/gtdejbgyni.html

[G07] 调用父类方法
来源：http://hz.jyoumei.cn/gtjwrprcrm.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtvtnikdbf.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gttqakrial.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtinjmqent.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtffanetkf.html

Java: super.greet();
来源：http://hz.yj20258.top/gteolpkfhh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.andypj.xyz/gtgzhgjltk.html

Ruby: super
来源：http://hz.tanke756.top/gtafywvpcz.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtaitmcsxl.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtpsnqehnf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtqzfqjftg.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtuhetviha.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtgxxyrady.html

TS:   static f(): void {}
来源：http://hz.guowangkeji.top/gtnymfwpto.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtwgkhvnth.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtubhdihwv.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangtech.top/gtivxpiklp.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtywzhfaua.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtbdbgdyry.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydjk.org.cn/gtcrxvanxj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gtsnbqindx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtdaitspvt.html

TS:   interface Shape { area(): number; }
来源：http://hz.cucudq.cn/gtelkscjps.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gtxwtfthbn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtwlbkjtlm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gaohongyu789.top/gtgiukibtb.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtvdvdogsc.html

[G10] 访问控制
来源：http://hz.jinqigufen.top/gtzbcgbgrp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtzbvxuiyx.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtdmxrhqoz.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtlgiaksnm.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gttmggmcxy.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtgqaolvft.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtushimiki.html

Ruby: public / protected / private
来源：http://hz.nwbrower.top/gtfqsolekn.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gthxjntbzp.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtusapsouj.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtdwkbtnvn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtdqaldwee.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtwvbzcgrm.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtizxghvaw.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtarcbtgvh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtwmkojqmv.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gttoycgfrs.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtinbhnhzh.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtjesouacr.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtctygjztx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtrjptsjgn.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gterbuaien.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtvnjrpqhp.html

Java: @Override public String toString() { return name; }
来源：http://hz.smart0.xyz/gtzmihxnkv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtmbsnscvh.html

Ruby: def to_s; @name; end
来源：http://hz.c1oappe.top/gtsdzeechk.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gtfyhopqbk.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gttuizylcr.html

Py:   isinstance(u, User)
来源：http://hz.dianchejie.cn/gtqjwxccbh.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtcrozlals.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gtwpubvqfh.html

TS:   u instanceof User
来源：http://hz.andypj.xyz/gtwzemcrve.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtszvsljgj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtcpdixelt.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gthuwldmfq.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtrjzwtwyy.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtnymvhnld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xziqi.cn/gtvrdprstq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtcgbjmalw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtifxjafuf.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gthywjqmlr.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtgqcpjyjt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258.top/gtpswqlbov.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cashguo.top/gthhjslxoj.html

C#:   record User(string Name, int Age);
来源：http://hz.xuetiantiany.cn/gtmxbuifmi.html

[G15] 枚举
来源：http://hz.316326.xyz/gtqvimlgue.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtssdxgylo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gtflaeabfl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtnkcvmtxf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtrdtjthal.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtjursskta.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnqzz.top/gtfyoxejaa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtjcxdivaa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtqmgkdife.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtjnzwgodc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtdixvklpw.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtslplhdwb.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtdvbvuiwc.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtsokbltvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtnjvngqro.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtjnpipbem.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtlrvtuqnk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtdjizelwg.html

================================================================================
来源：http://hz.hnqzz.top/gtgjdxiuor.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtijjkjzuz.html

================================================================================
来源：http://hz.ppjwa.cn/gtdofflyka.html

[H01] try / catch 基础
来源：http://hz.haohaochexian.top/gtenfxfqom.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gtjwhtabfg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtpmjoxrpy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtiidhmpjs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtfujdjiaw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtonwqvngi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gttnayzjmm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtwqoyxqtu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gtcfefiuci.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gttpnwgrwd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtpebgbutz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtlybqanlp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gttafppiku.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gturqtryql.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtjjmvlqea.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gttoennpaj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtqabdlnca.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtvuzurmbf.html

[H03] 主动抛出异常
来源：http://hz.andypj.xyz/gtnkqwqybz.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gtuofrobcu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtlwgqnxji.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtmcwcfqwh.html

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtvoosdxqz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gteqfiotpq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuanzhike.top/gtdtmhbgkr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.feifeiyinyue.top/gttacuvjir.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtjbtyxfxo.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtlekucmpi.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtwzxvcikm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gtosufsrnk.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtulrlkmbj.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtrggwhrmx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258.top/gtqbxjmreu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtggjedahx.html

Ruby: class MyError < StandardError; end
来源：http://hz.yvedp.cn/gtbacdugdl.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtjkzhjjdw.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtvuijhwob.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtejsgtikf.html


<!-- 参考信息 -->