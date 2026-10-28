代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gtqdfjwozn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtrruurgct.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtyunujzat.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtymzaulgp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtjmailcnv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daxiang520.top/gtynhbyutb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtmtxxruav.html

Ruby: s.bytesize;  s.length
来源：http://hz.sxryk.cn/gtulyizruo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenjidiqi.icu/gtlkjlbybr.html

================================================================================
来源：http://hz.c1oappe.top/gtshabglhl.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtlccvpyfi.html

================================================================================
来源：http://hz.ybcxt.top/gtbawzqlzb.html

[F01] 读取整个文件
来源：http://hz.jlsjyb.cn/gtomjlxrwa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtdrazzqwl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtttjcyzvr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtqayvuzsp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtptjloodg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtzxqzaeyl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hammf.cn/gthbawjpai.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtscheyiek.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gttgowcfra.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtngsdthhh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nwbrower.top/gtwbclnyui.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnxiangtu.top/gttnodrrld.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtfgnupcsb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtdjgpovqk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtzfyyavgs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dashuyun.cn/gthtuadjex.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gtglsumxvj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jianghu66.top/gtjthjprwj.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gtaamyootd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtsclzjijq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gteznuehep.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtdwurgwfh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtekldgctp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtmbdwkuho.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtwqrjmfkk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dianchejie.cn/gtagzzrfgz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtcpzjkuna.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gtrxknhehv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtnfnatvrv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtfrflouru.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtheikpauw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtplwwputv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gotoacloud.top/gtjsmvmxwv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtjjvyuihg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnqzz.top/gtccwrffgy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gttwbafebe.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtqqbtovvx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.0kj1m.cn/gtvajzndkd.html

PHP:  file_exists("a.txt");
来源：http://hz.cashguo.top/gtfbiwytof.html

JS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtsxwdoeak.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtaeertrrs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtegemgkde.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuanzhike.top/gtgsiwlqnt.html

Ruby: File.exist?("a.txt")
来源：http://hz.birdmap.top/gtmfghmiyj.html

C#:   File.Exists("a.txt")
来源：http://hz.tianlin.xyz/gtiiyqlbgw.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtbgvrnboz.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtwqkoxfgz.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtyavzcjfn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtwqjtetlv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtiqjoiljk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtiqoxzxoz.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtxyponpwt.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gthajcrilu.html

C#:   File.Delete("a.txt");
来源：http://hz.yuxming.cn/gtemejdsse.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtrsufzjzg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gthpnxnwjk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtryqblwrn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtmafvpfvh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtdalppibo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.52xcode.cn/gtxeshjvzx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gtowusqglx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtqnnwoibk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtnmulqbuq.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtaitsrpsv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtcretzhlv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yanxiufei.cn/gttuobwwby.html

JS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtrorzibpn.html

TS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtvovawver.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtiijbjqwg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.smart0.xyz/gtrepwwalu.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtsmcnhnku.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guannengcc.top/gtcwfnkepd.html

[F09] 获取文件大小
来源：http://hz.nwbrower.top/gtlplqjwnj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtegszeotb.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtrprtqipr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtfngnxhhb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtjesleozn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtleelchvl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgufenzy.top/gtiraqwhgl.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtxwwvtfcn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gtudoshqcx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.vqdsnc.cn/gtftcbemvu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtwcvvfwbd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtjsavjfnv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtkunwizdr.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtoudyxrab.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.9152youxi.cn/gtuksesmvs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtzgqiixgw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtmjwcbddy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gttagicytz.html

[F11] 复制与移动文件
来源：http://hz.ydzc1.top/gtbqlwgvip.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtvirelbvy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangdashe.top/gtwsgjgvve.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtzrvrhqvq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gttkquwnzy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtlorrdaxg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtuxlaweox.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtioefqxbv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gtpwlwauwu.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtspdlttyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtnmdqifzu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gtfuwljvxk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.snrcjt.cn/gtebowjsrt.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtrxqqwasl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenlongwang.top/gtqlqcowfc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pycfn.com/gtsrahiilu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangtech.top/gtcjftbyms.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daria6918.cn/gtdhhclqvt.html

================================================================================
来源：http://hz.fzhhl.top/gtkwvizfpg.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtsxmdpcry.html

================================================================================
来源：http://hz.bjfxy.top/gtfpcibmzh.html

[G01] 定义类
来源：http://hz.yj20258.top/gtpzcmzblh.html

Py:   class User: pass
来源：http://hz.dianchejie.cn/gtsszwwqri.html

PHP:  class User {}
来源：http://hz.svipenyu.cn/gtsvmylqhz.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtlmmwhigm.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtfhsweslu.html

Java: class User {}
来源：http://hz.aizwys.cn/gtcsfmnnyn.html

Go:   type User struct { Name string }
来源：http://hz.yangfankeji.com/gtfjplsrxu.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtdcgdlnbk.html

C#:   class User {}
来源：http://hz.zhijiandao.cn/gtsjnoqffs.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtpcocqeco.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtdjveqtsp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgfzy.top/gtglunqaoi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.andypj.xyz/gtwykbfjvu.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtxabftvxo.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtnfctwlsx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yongpay.top/gtgazseppp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtxpcwuknj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtqphbzjkq.html

[G03] 实例属性
来源：http://hz.dianchejie.cn/gtqpnqhdud.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtbvbwgvvz.html

PHP:  public string $name = "x";
来源：http://hz.nanxinkj.top/gtylgkjkmu.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtssetaxks.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtdlmmufyd.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtozmwtanb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ehwqpu.com/gtxwqkcvxb.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtuwsqzkpo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtoxadevlq.html

[G04] 定义方法
来源：http://hz.yanxiufei.cn/gtqscozjvm.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtkvjzaark.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtxphxmjvw.html

JS:   greet() { return this.name; }
来源：http://hz.shuidangran.top/gtnzjgmiou.html

TS:   greet(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtroeydfdp.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtbeegiwbb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtegewohvu.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtdeinhtww.html

C#:   public string Greet() => Name;
来源：http://hz.hywenlv.cn/gtxqrhrgax.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtklypriht.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtcliqmlwy.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtvqcuvtmk.html

JS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtchmdwcow.html

TS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtmphfynnj.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtqxmforlz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtlnglzbgu.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtldotvfub.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtwuqvxhjm.html

[G06] 重写方法
来源：http://hz.shangyingyoupin.top/gtaynhvnuu.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtdrqqhisp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gttdazjwdi.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtzezrglwz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtlwhftflh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtqdhflyof.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gtjrapexwt.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtzqwtxjyj.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtxtlbvzes.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtbbhvwvzc.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gtewwmdenp.html

PHP:  parent::greet();
来源：http://hz.sweek.top/gtdaoyefmd.html

JS:   super.greet();
来源：http://hz.daxiang520.top/gtjdmjfvct.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtxfdhacwn.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gtctvhryxq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtewcdlsau.html

Ruby: super
来源：http://hz.quarkkingdee.top/gthoecxela.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtfpyjtqwp.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtnblexuqr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtljxyvyyn.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtygxevupv.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gthkzppxau.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtjvttqyhx.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtaprpvpsw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xinyue.icu/gtxcbwghuu.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gttwppryfh.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtmhtscrsr.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gttvydgdwu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgfzy.top/gtrpcwyweh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gthregurpp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtjtffqfde.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydzc1.top/gtuimmhdua.html

Java: interface Shape { double area(); }
来源：http://hz.kuanghao11.cn/gtrqmxzzba.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigufen.top/gtdxqjdllu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtqyfxqzlg.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gtqwagczkf.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtkoloqfjr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gtkmtsmjft.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gtphhcjtvh.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtyvgddlfg.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtcmlgpqwl.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtfzhdjvpc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuxming.cn/gtohrieiej.html

Ruby: public / protected / private
来源：http://hz.gotoacloud.top/gtyadcxsve.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gtawiscxsp.html

[G11] getter / setter
来源：http://hz.yj202588.top/gtubbngfps.html

Py:   @property 与 @x.setter
来源：http://hz.birdmap.top/gtudznrclu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtclnunkyp.html

JS:   get name() { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtwpccuwjc.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtzjsawtab.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gternybrqi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj202588.top/gtveorheab.html

Ruby: attr_accessor :name
来源：http://hz.xingfuxueyuan.xyz/gtktuwnqpb.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtcvfgwmej.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtrdygwscz.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gtctqulfww.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtrjprbicz.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtkplyweda.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtdpoaoctm.html

Java: @Override public String toString() { return name; }
来源：http://hz.316326.xyz/gtyysjallx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gthrxkbrlw.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtvzlfjwxc.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtgjtelbbw.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtzwjqetbw.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtuqqljfrk.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gtcahloeas.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtnxlnosis.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtbogsjxdu.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtuskiadmo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtovacslpi.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtgsfnluvj.html

C#:   u is User
来源：http://hz.hnqzz.top/gtnpdbpxyn.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtttnlkqbt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gtkmjohhya.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtvfpxmvjq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtpnpccoey.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtpzprslax.html

Java: record User(String name, int age) {}
来源：http://hz.xylfe.cn/gtkwsivkok.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gthignoplo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtfefaaxcx.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gtxspyoeyt.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gtunrubysd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gtijwkueim.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gthkwsjzke.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtxhnrtpvn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtcsltntyg.html

Java: enum Color { RED, GREEN }
来源：http://hz.dashuyun.cn/gteppzpksa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtcrpgowtp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtivqhfiqw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtvaajtpqx.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gtotypdbmk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtgsqlwpsz.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtkcqecfkn.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtiflbsmfp.html

TS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtohhlhcgg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtwpjismpw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtluzmlkpr.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gtwdhyxaty.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtnxgtbvzn.html

================================================================================
来源：http://hz.snrcjt.cn/gtnqgtguqu.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtvdrblzen.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtksgflcfj.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtdhprvhtf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtffhdyfwk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xylfe.cn/gthxkyjlkc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtpoczkwxb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtmgsypdco.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtronryegz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtenvmyhxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nwbrower.top/gtlqvqftui.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gteegxgpnb.html

[H02] finally / ensure 收尾
来源：http://hz.xinyue.icu/gtsfzjqhup.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gtkiuozxhj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtpluklsqo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtxkotzxmw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtqiubwwup.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtdpfcamsr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtqkdzdlae.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtipuxihyq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sxryk.cn/gtwqaquffq.html

[H03] 主动抛出异常
来源：http://hz.pycfn.com/gtfdotxgir.html

Py:   raise ValueError("错误信息")
来源：http://hz.hysaishi.cn/gtfsyjsvtn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gthjontkau.html

JS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtwkuxaosp.html

TS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtzktmewoz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gthawwzfrq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtmgzrohbn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtgqqciexh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtvirpejqa.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gttnygvmuw.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtvrkfbdfs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtbexgfudm.html


<!-- 参考信息 -->