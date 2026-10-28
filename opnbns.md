代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtlytqrvlu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ywan-chungtsiang.top/gtlngeeuiv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gotoacloud.top/gtzmvvydjd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtihpifxro.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigufen.top/gttzcifehc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gtezlcfykz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gtahdikbpi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtxsxrpmyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtnarylukt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtkmdjhoas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yueranfly.top/gtchlgljir.html

Ruby: s.bytesize;  s.length
来源：http://hz.feifeiyinyue.top/gtavopdgeb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtmvyoutrv.html

================================================================================
来源：http://hz.mhx1999.top/gtmlhosgbl.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtddukcoyk.html

================================================================================
来源：http://hz.snrcjt.cn/gtjyyigsor.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtatpgohzv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangdashe.top/gtcttlvoyc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtnbavsamm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgfzy.top/gtogmacamg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtlucqmfys.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtqtllxdow.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gtvxeookvi.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtecpxyyai.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtzrmsogln.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtiudgusrz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtiibtzjtp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gthjccowkd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtihdckjzh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtplufjblf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtmmahpckj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hfpthk.cn/gtynzowsfa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hongshengwenyu.top/gtjyyafuun.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gthfqqwwcc.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtccggxtpf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gthbigfvma.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtpaakaodz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtipgmxdyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gttwyaidxg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ehwqpu.com/gtesumlqkl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtlcwafdin.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.kuanghao11.cn/gtxsiwfrjv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtryptkyyu.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtqtnzppjd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtzmptbcav.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtnkfcwqct.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtooyipuon.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtqcdtbjto.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gtqlbodehu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtikrrbjtk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jlsjyb.cn/gthxzthihk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtnlkndahh.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtqhtmrdnd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtayqerpqb.html

PHP:  file_exists("a.txt");
来源：http://hz.cheryme.top/gtgalgiyqd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtpjnwfheg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gthjjfuccl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtxosozboz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtcsomeqgx.html

Ruby: File.exist?("a.txt")
来源：http://hz.dianchejie.cn/gtvdpopssb.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtvvnlrwaw.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtnedkhmzn.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtjihtqdkb.html

PHP:  unlink("a.txt");
来源：http://hz.gotoacloud.top/gtqnzbjept.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtdmrjgixk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtqycoxxyu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtsflqpmak.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gtydopfyrd.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gtptoalkgl.html

C#:   File.Delete("a.txt");
来源：http://hz.bjfxy.top/gtlcqdvgaj.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gtuxxukltx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtramdbypw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.c1oappe.top/gtzxebxxsm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtrztlynhb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtvlqtczct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gtsmkcfzpf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gtooldevrc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtoppwpjfg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtfeerowap.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gticmhjjgs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigufen.top/gtposdtkui.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gtgqdrknzo.html

JS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtqlrvvgrd.html

TS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gthabhvqtg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtvgnntcsg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtdojdnzbs.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gthydycjjm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.vqdsnc.cn/gtevrpflla.html

[F09] 获取文件大小
来源：http://hz.yj20258888.top/gtxcghrmlt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shuidangran.top/gtarnybirv.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtqwgopvsw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtwhoaodcw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtevkyxjyd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gteviuchgf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fzhhl.top/gttkvlhzur.html

Ruby: File.size("a.txt")
来源：http://hz.gzhubu.top/gtiubmqwjm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuanzx.com/gthflbsswc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtupjpzdrx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gthgmzahrx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtnctgifxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gttgerdvtu.html

TS:   path.extname("a.txt")
来源：http://hz.fzhhl.top/gttwlhhtat.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aizwys.cn/gtjndgdvso.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtwndmwrzm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtjpynmwlk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtchmfxleu.html

[F11] 复制与移动文件
来源：http://hz.wangshuangyany.cn/gtfzssdwia.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtmbikwhrq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtgixxoegy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtqqvgsdam.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtxkcnvorg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.bjfxy.top/gtotrgqgsr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtervenwfq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtipvabssr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtdjedzams.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gteirfrpld.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hammf.cn/gtucwtcito.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtlkeysqmu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ybcxt.top/gthdaqtkqs.html

TS:   // 同上
来源：http://hz.birdmap.top/gtpjwjwxaw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtbtoieuyn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtvfphuafb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daria6918.cn/gticjkxszt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.0kj1m.cn/gtwomifbnv.html

================================================================================
来源：http://hz.daria6918.cn/gtlzeyljjw.html

G. 面向对象
来源：http://hz.yangfankeji.com/gthurpyaev.html

================================================================================
来源：http://hz.jqgfzy.top/gtqzfasyuv.html

[G01] 定义类
来源：http://hz.zycfv.cn/gtyarwpdgd.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtileogyph.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtknwftlby.html

JS:   class User {}
来源：http://hz.kuanghao11.cn/gtodkkcqkl.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtqmtxbdhl.html

Java: class User {}
来源：http://hz.nanxuanxn.top/gtxqrighet.html

Go:   type User struct { Name string }
来源：http://hz.mhx1999.top/gtmacipztn.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtfpiccirc.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtcykcltzk.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gthtcylmwi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtlwkvpkfz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtmpwfwgjk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtukejrtlp.html

TS:   constructor(public name: string) {}
来源：http://hz.xinyue.icu/gtiwlfohrs.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtatjwvess.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtlkfvpezq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtngzsocxz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtmyqwajdh.html

[G03] 实例属性
来源：http://hz.nwbrower.top/gtlrkhkgoy.html

Py:   self.name = "x"
来源：http://hz.cqqwz.cn/gtniuryxra.html

PHP:  public string $name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtyxlyidrl.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtncfmnneg.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtgpnhxgtn.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtydbhkdwd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtkacylbpj.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtpdnfstft.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtgiwmcukd.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gtnyvwjasp.html

Py:   def greet(self): return self.name
来源：http://hz.gaohongyu789.top/gtuyvqbqdx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtdscrzhbv.html

JS:   greet() { return this.name; }
来源：http://hz.mhx1999.top/gtewhvcpgy.html

TS:   greet(): string { return this.name; }
来源：http://hz.mhx1999.top/gtmpqenklr.html

Java: String greet() { return name; }
来源：http://hz.haohaochexian.top/gtvkynzxwa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtohbvjueq.html

Ruby: def greet; @name; end
来源：http://hz.sweek.top/gtspslchim.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtkxhbtzey.html

[G05] 继承
来源：http://hz.jqgufenzy.top/gtudvanjvh.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtocanfefk.html

PHP:  class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtakjhadso.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gttmbdydem.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtfyepiwpl.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtwwdfezzw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtxbzfabxx.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtaiezsclv.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtwnjmnsln.html

[G06] 重写方法
来源：http://hz.zhengqikj.top/gtbuoivhlw.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtbtdknonc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gthmiwufqf.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtkiqsmbzj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gteazpydlo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtoxwtuibu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.quarkkingdee.top/gtywifcwum.html

Ruby: def greet; "admin"; end
来源：http://hz.gogol.net.cn/gtmobzawkn.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtdcyokojm.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtfepepndk.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtmfprnwfa.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gtgkzxmlli.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gtzejyuwps.html

TS:   super.greet();
来源：http://hz.sufxvd.cn/gtttkpmcwz.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtrowyesus.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtykvkxhzf.html

Ruby: super
来源：http://hz.fzhhl.top/gttinywhtt.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtahsxrfzc.html

[G08] 静态方法与属性
来源：http://hz.yj20258888.top/gtvuxmixhp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtsfaunmjv.html

PHP:  public static function f() {}
来源：http://hz.tian-w.cn/gteawwpdrc.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtiuyodmyq.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtfnjlbhzb.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtsnjxtdtu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.svipenyu.cn/gtyingehqn.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtkzhzmlks.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtrgrihpcs.html

[G09] 接口 / 抽象类
来源：http://hz.zhiwuduotai.top/gthqitpuyn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xylfe.cn/gtdonxyeru.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.mhx1999.top/gtozxynqiv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydzc1.top/gtvdzppckq.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtyxiqbwfa.html

Java: interface Shape { double area(); }
来源：http://hz.yueranfly.top/gtqgcavhgq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gtvinmspjk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtgvkyghkl.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtfmmllgze.html

[G10] 访问控制
来源：http://hz.shangyingyoupin.top/gtontgxevj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gtnpeyrgsj.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtfbmraddv.html

JS:   #private 字段；其余公开
来源：http://hz.xingfuxueyuan.xyz/gthhxcmbin.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtvadznpxv.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gtjhoucjqq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtktvdfzzd.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtskbmwkbr.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtwwmynokz.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtcyflmnhs.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtsqcxabcc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtucwumgbj.html

JS:   get name() { return this._name; }
来源：http://hz.hywenlv.cn/gtbcnztwdt.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gtqxlufjxo.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtnfuswqxo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtlfbgzllx.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtvubnjnpa.html

C#:   public string Name { get; set; }
来源：http://hz.zdqjudy.top/gtkaarkpfj.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtjbespild.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtgjfhqkzr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gttcxwixjk.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtyzatsvoe.html

TS:   toString(): string { return this.name; }
来源：http://hz.haohaochexian.top/gttjvdjako.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtdfhinasf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtwehhlbkd.html

Ruby: def to_s; @name; end
来源：http://hz.iojbl.cn/gttsgsoiun.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gtztfsrhqj.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtdjgpkyre.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtoozrgpfj.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtwnznmzzh.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtswbpgdaa.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gtdtqoxiaj.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gtammdhjvd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtgntrmxwa.html

Ruby: u.is_a?(User)
来源：http://hz.xingfuxueyuan.xyz/gtojosjnwn.html

C#:   u is User
来源：http://hz.0kj1m.cn/gtffqcnxhr.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtpjpimldx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtzoespkiw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ehwqpu.com/gtpcpfrtyt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtkmmvieww.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtgbterehk.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtankknlvp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtqhkknyzz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtxmycbkom.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gthrqydosg.html

[G15] 枚举
来源：http://hz.bjfxy.top/gtxqoskshj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ehwqpu.com/gtvttahjaa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtadtrkuot.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.smart0.xyz/gtnvesckxh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtivvpswdh.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtnixmjjlj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.52xcode.cn/gtvebuwvqj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtwbktwmnv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtubxlwoeb.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtmeaujxci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.havefunace.top/gtogljwvpo.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gthskhkwqr.html

JS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtkokjfubj.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtoffgvzso.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydjk.org.cn/gtonyjxyxb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jlsjyb.cn/gtaguluctr.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtnwnluaxs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuetiantiany.cn/gtigzxcaxu.html

================================================================================
来源：http://hz.dashuyun.cn/gtxqqgvmov.html

H. 异常与错误处理
来源：http://hz.ydjk.org.cn/gtkyppsfrj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttwyljjvm.html

[H01] try / catch 基础
来源：http://hz.jinqigfzy.top/gtinlgbbiu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtkqxaksme.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtxaapaoip.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtrqpnrxcm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtsorfbyuo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtiduyteyh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtrdejjmxb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtskawskdm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtuvkfgpxj.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtywtnwgnd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtdeuksbrq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtntqutned.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtshbrsgxw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtqniusxab.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtdfqimthw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gogol.net.cn/gthcgftyhl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtpxgwfzxc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sweek.top/gtlskqxivx.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtzhlaesve.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtxkbhrliu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtkiahysfu.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtepbnczxn.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtuamyptqn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtsqlpstgu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gtcjthvgjt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gtxfqnoqad.html


<!-- 参考信息 -->