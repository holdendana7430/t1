代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gttrasaxcz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtrqxdtacc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hongshengwenyu.top/gtbbhiyzic.html

Ruby: s.bytesize;  s.length
来源：http://hz.cheryme.top/gtyffsveuf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtyinduobr.html

================================================================================
来源：http://hz.zycfv.cn/gtocpbsmnj.html

F. 文件与目录
来源：http://hz.dashuyun.cn/gttxwgcxes.html

================================================================================
来源：http://hz.ehwqpu.com/gtlcokkwjq.html

[F01] 读取整个文件
来源：http://hz.xinyue.icu/gtisyuntqb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.redwolf501.top/gtuorgndgv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daria6918.cn/gtdkuarxpd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtesanozkb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gteyvratbd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtyinyzbgd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yonumen.top/gtnzcaxmjn.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gticorguhm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258.top/gtbbxsyaqa.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtjujrlioi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gtwblzyozl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtkxiuwzlb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtsiubllcw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtzkbzkyky.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtyrklialn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtcaznxtmz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gtxtvqgont.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.iojbl.cn/gtmtuhgzhk.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtmkubhvnk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtaoplxpkc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtwsykcwfz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtlewhilse.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtlzpxwzib.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtonqqrjyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtujjwhtvs.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtploutrld.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtwnjlhexp.html

[F04] 追加写入文件
来源：http://hz.yongpay.top/gtbuyntcbi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgfzy.top/gtfkpjkwsb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ivvv.top/gtpeuakrdp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtrvlaeqdc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtanhnigol.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.svipenyu.cn/gtpiuftvhn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtncotvodl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangkeji.top/gtmkizuuda.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtefmfrwpk.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtviyamlps.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtzyzrkxst.html

PHP:  file_exists("a.txt");
来源：http://hz.daxiang520.top/gtbszifemy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gthhxvhkdn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtdumamdls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtiyyyhrsi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtqasgxmtq.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtekagxurk.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtcvqiksym.html

[F06] 删除文件
来源：http://hz.haohaochexian.top/gtybdgasla.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtinotdtub.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtywgwktwl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtnukhfcjf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtsflgexdf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtzsdbmpen.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtnvwrciik.html

Ruby: File.delete("a.txt")
来源：http://hz.kuanghao11.cn/gtipacshco.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtllgfcelr.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtwilvipwe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtolnkkzuw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guannengcc.top/gtmuyxcjrt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtwkncgmni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtzmngjstw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuxming.cn/gtbtdgqebq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gtrwwggect.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtgamjggwt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shzxlz.cn/gtfpoqzyqh.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gtctcogvoj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtkxkuataw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gtcqfthofj.html

JS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtfcjxccuh.html

TS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtmsqjvtmn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtrhqbjoer.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtteaizcor.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtvfoslysw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtqttehbjq.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gtzlimskux.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nwbrower.top/gtzptwrrdr.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtqcpzzlzp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtjkacqnml.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtqzvnlime.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtgjschrzs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtzthisaan.html

Ruby: File.size("a.txt")
来源：http://hz.cdnleiting.top/gtpykbfyqh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtanmlkdgp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.quarkkingdee.top/gtpphuxuzy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtmqqcwyve.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtfxmdashz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtizbglzmn.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtrqxobrow.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtdogzopat.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gteqsdciul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtxomixuze.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gtcnobzezu.html

[F11] 复制与移动文件
来源：http://hz.feifeiyinyue.top/gtcpcmklvh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtikutbvfx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zycfv.cn/gtakfmtzei.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtqzxasqkb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtxzvhssjb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxuanxn.top/gtemvetrbx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gtqbleydru.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtxdamwakm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gthcnjlufy.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtevozhwmt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fzhhl.top/gtrutcxvto.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dianchejie.cn/gtmxeqhhkw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtzlzawixo.html

TS:   // 同上
来源：http://hz.birdmap.top/gtxzihqmyl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtpootflzv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhongyouzk.top/gtvpkvnzyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.haohaochexian.top/gtxevasbge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nwbrower.top/gtwtdmfxcz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgcjlkabm.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtdslipqev.html

================================================================================
来源：http://hz.jyoumei.cn/gtyocnzqtr.html

[G01] 定义类
来源：http://hz.daxiang520.top/gtpgpurktf.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtqmfeodav.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtjuoyotlp.html

JS:   class User {}
来源：http://hz.shanyushiyangtech.top/gtkadztcly.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtvgmhdbqh.html

Java: class User {}
来源：http://hz.jiagoushi.top/gthztgreka.html

Go:   type User struct { Name string }
来源：http://hz.haohaochexian.top/gtkltsyxsx.html

Ruby: class User; end
来源：http://hz.daria6918.cn/gtpschtccm.html

C#:   class User {}
来源：http://hz.zhijiandao.cn/gtfvigloiv.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtsuiqrwee.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtqjmqgils.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtfrastoca.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtyuztsrin.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gtkiiewqqf.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtbdaynkru.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtiqxeqlen.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sweek.top/gtiatvnjnb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.vqdsnc.cn/gtatmfrnvu.html

[G03] 实例属性
来源：http://hz.yongpay.top/gtmzgdejco.html

Py:   self.name = "x"
来源：http://hz.yj20258.top/gtajfshwjp.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gturueghhm.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtwjlogbab.html

TS:   name: string = "x";
来源：http://hz.hammf.cn/gtbkumlahs.html

Java: private String name;
来源：http://hz.shuidangran.top/gtzsxezmbf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangkeji.top/gtvfgibevk.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtgbpqhkto.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhijiandao.cn/gtjlipspev.html

[G04] 定义方法
来源：http://hz.haohaochexian.top/gtehklrtqz.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtnvhxwgmi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtjlvdorlr.html

JS:   greet() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtktmgloml.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtlbtmdfao.html

Java: String greet() { return name; }
来源：http://hz.aizwys.cn/gtcrtpblwr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtjpwpqcgc.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtmmmexkrd.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gtrlhiwkvp.html

[G05] 继承
来源：http://hz.316326.xyz/gtubqrannw.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gtpvtpgvtc.html

PHP:  class Admin extends User {}
来源：http://hz.pycfn.com/gtvnuuwcwd.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtozrbllez.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtjbtredri.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtbqwuzqid.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtrblezift.html

Ruby: class Admin < User; end
来源：http://hz.sufxvd.cn/gtvcaqldvq.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtjkqskgcc.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtxhkikavg.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtuocdcmqx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtozbvytde.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtzabiflww.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtaldirvzx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gthooadaxc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtysijnslt.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtlauopkgw.html

C#:   public override string Greet() => "admin";
来源：http://hz.pengpengdd.cyou/gtdqfbpoox.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtslxhyvnn.html

Py:   super().greet()
来源：http://hz.hysaishi.cn/gtvnwodqis.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtjzftxbjz.html

JS:   super.greet();
来源：http://hz.tianlin.xyz/gtudknpuca.html

TS:   super.greet();
来源：http://hz.havefunace.top/gtccnodfgu.html

Java: super.greet();
来源：http://hz.jlsjyb.cn/gtonmxdpgd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuetiantiany.cn/gtuhcpjvmb.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtunykkdle.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtlfqpyeja.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtzbniavnx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtrbhegfgp.html

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gtxidpzuoj.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtritzbuvn.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gtwlxmwalf.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtxmdjrowi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sufxvd.cn/gtmuvenqtt.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gttuoyuzbl.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtninranke.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtlilvcwfr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gtpwxslkvf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtrxivlfpe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtimoqnase.html

TS:   interface Shape { area(): number; }
来源：http://hz.haohaochexian.top/gtjyooqmfn.html

Java: interface Shape { double area(); }
来源：http://hz.jqgfzy.top/gtacovcuvh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtbbmnuesc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hongshengwenyu.top/gtoehdutzm.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gteagslyzf.html

[G10] 访问控制
来源：http://hz.haohaochexian.top/gtukbiiktz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fzhhl.top/gtvlxsurkj.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gtdnmeuegj.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtbjevsqer.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtlfhzcahf.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gtgizgkyhl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtvaxrusee.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtnnbslruz.html

C#:   public / protected / private / internal
来源：http://hz.redwolf501.top/gtavmfrfdh.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gthrjrbvra.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtnmgmyvmm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtnxjqmxtd.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtqeaarznm.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gttqmutbjm.html

Java: public String getName() { return name; }
来源：http://hz.nwbrower.top/gtpluaitzf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gtsqoiqxvu.html

Ruby: attr_accessor :name
来源：http://hz.hnxiangtu.top/gtxpdnclom.html

C#:   public string Name { get; set; }
来源：http://hz.yuanzhike.top/gtstykffix.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtnhkgwmfi.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtvrmvljlw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gthkhqutdo.html

JS:   toString() { return this.name; }
来源：http://hz.havefunace.top/gtposkbhsl.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtewwxbkpa.html

Java: @Override public String toString() { return name; }
来源：http://hz.redwolf501.top/gtpqaksnfn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtzwbvzwmn.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtwdwamznf.html

C#:   public override string ToString() => Name;
来源：http://hz.kuanghao11.cn/gtajkhdxtm.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gtswvpayjw.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtaictxxro.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtntzgpgru.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtbreznagt.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtfbcjxkic.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gtibxohkon.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gtbpbkuwwq.html

Ruby: u.is_a?(User)
来源：http://hz.hywenlv.cn/gtcuuhozvw.html

C#:   u is User
来源：http://hz.pengpengdd.cyou/gtfjgwicxp.html

[G14] 数据类 / record
来源：http://hz.yongpay.top/gtqhtzjuzs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtompborew.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gthjyguzkr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtjuvtpxxe.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gttdcmtduf.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtpcqxpnre.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hysaishi.cn/gtlseffdkn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtmubejtjk.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtolutamzq.html

[G15] 枚举
来源：http://hz.zhixingplan.top/gtpfynnysh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gzhubu.top/gtchggbutp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gtjgzatdou.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtlxmwcazb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtnutklpru.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxuanxn.top/gtibnzpper.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cqqwz.cn/gttrskiuil.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtcdonlvmk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gteyytmhkl.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtcuqdtyua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtbdunlhwp.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtkzpvlyiy.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtfsbavfwr.html

TS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtjgymwxfc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.birdmap.top/gtweutpwiv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gtrdhaifdh.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtjupdwyta.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtffejrlvo.html

================================================================================
来源：http://hz.c1oappe.top/gtsecgtvty.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gtaqduojin.html

================================================================================
来源：http://hz.yangfankeji.com/gtgkawqejc.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtjqfktupa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtojioowgz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtzwhiwxem.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtbntoivdw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtowpaczgx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gzhubu.top/gticudveob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yvedp.cn/gtjqhalvis.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.feifeiyinyue.top/gthsepquly.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gtdcmhfwnl.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtyuwwegck.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtsxgcgthr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtzbqskpxy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gthvyhpsyl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gthwqlzwty.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtgdzxcjjd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtuclcfqlt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangshuangyany.cn/gtdrldwvwl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtbcuigldv.html

[H03] 主动抛出异常
来源：http://hz.sweek.top/gtxccvxrrq.html

Py:   raise ValueError("错误信息")
来源：http://hz.iojbl.cn/gtotvcjjjg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtpkcvxmnq.html

JS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gttctpidzg.html

TS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtngjequoi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtmuzocayn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gttaellxum.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtdfpvzkbe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtxbyfyugt.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtvvgjzmua.html

Py:   class MyError(Exception): pass
来源：http://hz.haohaochexian.top/gtbatngxhv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtcfagjhbw.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtyeekeuch.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtxvuuysox.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtvyyyhidn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtvgjkzcli.html


<!-- 参考信息 -->