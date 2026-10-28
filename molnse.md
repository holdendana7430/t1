代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtihxedjlm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gogol.net.cn/gtfkihdgvu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtygtrveel.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtdwnxhfqr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gttiycuvhn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtyygyhkvz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zdqjudy.top/gtvvcwgzzd.html

Ruby: s.bytesize;  s.length
来源：http://hz.cheryme.top/gtcfjpteij.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gtkfqbyxml.html

================================================================================
来源：http://hz.guowangkeji.top/gtlcpbxasf.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtdsikecwy.html

================================================================================
来源：http://hz.hysaishi.cn/gtnfnpoylm.html

[F01] 读取整个文件
来源：http://hz.yj202588.top/gtoizldxbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtapsifhbw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtbhuovqvv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dianchejie.cn/gtpjmsbxlw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gthxmbeezp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtathlysdw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jyoumei.cn/gthcldayzg.html

Ruby: File.read("a.txt")
来源：http://hz.jlsjyb.cn/gtauggfsud.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtvusweqvg.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtfjdmxprk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hammf.cn/gtpxkkguun.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtyobfvcwg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gteyiqhxdg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtxhqyubcu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtdzrsrkbh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtkoubvkmo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xingfuxueyuan.xyz/gtatyhgjsw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guannengcc.top/gttrluxnha.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtlierubxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtsywmimwh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtkbjttjuq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtnsnqdqny.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtwnewndyz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gtnerygisn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtsefpmshf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtwzkybrxw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shuidangran.top/gtqvvgiknc.html

[F04] 追加写入文件
来源：http://hz.ywan-chungtsiang.top/gtjiimfrxa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gtgknamazz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gteesqlcpl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtwlaaukvk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtnbfmqelm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtvyalzulr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sweek.top/gttahqkyxe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydjk.org.cn/gtgkwnvakk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aizwys.cn/gtvvozolba.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtgxzafqhy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jlsjyb.cn/gtlxuujgor.html

PHP:  file_exists("a.txt");
来源：http://hz.cheryme.top/gtmkwextio.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtounnrpbd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtfmckwhfp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtxnmvqxpz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhongyouzk.top/gtwptynfsy.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtyxdguymp.html

C#:   File.Exists("a.txt")
来源：http://hz.ydzc1.top/gteantojoj.html

[F06] 删除文件
来源：http://hz.ppjwa.cn/gtqeosnbnq.html

Py:   os.remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtvkwmrtls.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gttftatihs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtckutwvwg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtdoicycfh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtauevisoh.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gtmlgqacsn.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtxkbshgsv.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gtuxlqfgjx.html

[F07] 创建目录（含多级）
来源：http://hz.c1oappe.top/gtdbzscknr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtayxknnot.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtuumphgbv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtuypehagz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtfnhlnsyd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtestcluvn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtkvmklgrl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtzuypdlvf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gtsutlryyq.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtsqglyxnh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtqghbqkbu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtwvfmetlu.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtriuqdhsx.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtphhzeole.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtgudlanzh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fengsongda.top/gtmjmqdruy.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtqbojdpvf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydzc1.top/gtueznsdri.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtouuuttdl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnxiangtu.top/gtmfzxvnfa.html

PHP:  filesize("a.txt");
来源：http://hz.havefunace.top/gtnbluuvug.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtcptmdhbg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtelefciez.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtrxudjmnh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtwvefhwmc.html

Ruby: File.size("a.txt")
来源：http://hz.zhengqikj.top/gtdwxohrcz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gtmsysxtnc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gtaoaokwyc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtantoibmg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sweek.top/gtydldzhgu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtqkkfeywd.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtjtirzemm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtvwbpswzt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtdlxcydvg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtbcavdzgi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gthwwpnqew.html

[F11] 复制与移动文件
来源：http://hz.jinqigufen.top/gtooixrelp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtefdllkri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgufenzy.top/gtrrejexfg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtlofljoxz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtxrxkosbw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ybcxt.top/gtxttqfqxb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.svipenyu.cn/gtktuvsqpu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtuldmgorq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yvedp.cn/gtkmaignpf.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtgorfteiv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhoulong.xyz/gtewjvsdyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gtkedsmegy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daria6918.cn/gtkgszjjon.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtlgqwjszu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aizwys.cn/gtawqvfdcu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtowwawhwe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhengqikj.top/gtaznoixuc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pengpengdd.cyou/gtydjwthyn.html

================================================================================
来源：http://hz.jianghu66.top/gtjhnlanor.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtbkwzeezt.html

================================================================================
来源：http://hz.sysykeji.top/gtgwuzrndv.html

[G01] 定义类
来源：http://hz.birdmap.top/gtdjisklxn.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtgwruvsoq.html

PHP:  class User {}
来源：http://hz.wangdashe.top/gtfvlntlsd.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gteokgcmcr.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtzkmwxhit.html

Java: class User {}
来源：http://hz.nanxinkj.top/gtqasggftz.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtoyedusdw.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtwibiqagc.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtctwqiiwr.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gtfrgjgpge.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtpsxobxuq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtbzrscvny.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtgqwkkryz.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtpblwkmhh.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gtxdozdchs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dianchejie.cn/gtdathyyyf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sweek.top/gtotznmyfd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtxeqyhsoi.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtxvlfyhct.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtqgragjsc.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gticgqbtyo.html

JS:   this.name = "x";
来源：http://hz.gaohongyu789.top/gtnjbqjqtn.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtqjlujenm.html

Java: private String name;
来源：http://hz.jyoumei.cn/gtthjpikrv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtkxoevdam.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtoovbkwim.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gzhubu.top/gtiebrmrio.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtepbfbbqd.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtppycjzat.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtjguqpzcm.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gthiegfkif.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258888.top/gtccwsvkaj.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtxmqtuuin.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtrikgtuar.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtjqhpavrq.html

C#:   public string Greet() => Name;
来源：http://hz.xziqi.cn/gtranlpomt.html

[G05] 继承
来源：http://hz.yongpay.top/gtiwnptfhu.html

Py:   class Admin(User): pass
来源：http://hz.nanxuanxn.top/gtefgerqwk.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gtglocfyiy.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtfwqabhmi.html

TS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtsutwrhqp.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtmfpzgphr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhiwuduotai.top/gtwfeqdkbx.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtstbrylnq.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtksnuinzc.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtwdxerolj.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtfdlukdfb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtvqruwzcv.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtkalqjdwx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtavoytvds.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtvzvkcgzc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtorgluiqv.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtgkkyzmxx.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtapvlirww.html

[G07] 调用父类方法
来源：http://hz.chenlongwang.top/gtsyrubips.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gtyfqpbtdz.html

PHP:  parent::greet();
来源：http://hz.nwbrower.top/gtonkgwuxy.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gtoeiiyzse.html

TS:   super.greet();
来源：http://hz.meibo888.top/gtxnjcgfvs.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gtotwznxkp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gthyyswpdb.html

Ruby: super
来源：http://hz.xylfe.cn/gtxwqvskcu.html

C#:   base.Greet();
来源：http://hz.ydzc1.top/gtrxdmclmt.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtdeiwwufc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.havefunace.top/gtdzblaiib.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtteqmrdoi.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtqnglhgec.html

TS:   static f(): void {}
来源：http://hz.shzxlz.cn/gthevumwkc.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtzryfxakb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gturvenoxg.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtyfvunwah.html

C#:   public static void F() {}
来源：http://hz.andypj.xyz/gtvgjcsmeq.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtjspyauqw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtwsnflkzj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.havefunace.top/gtilzdmpxi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtnrfwvgxd.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gtxzetoyme.html

Java: interface Shape { double area(); }
来源：http://hz.yueranfly.top/gtmzdxfcsc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gttwrpdulu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtcvgxeplw.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gttubxkzot.html

[G10] 访问控制
来源：http://hz.tianlin.xyz/gtnvdobobi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ppjwa.cn/gtlmtqagwt.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtbkeekeqe.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtkwnxlfgk.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtrntqfcvl.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtvayegnnp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtnphibfqi.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gtagjylftz.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtwsfbursm.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtgsspaces.html

Py:   @property 与 @x.setter
来源：http://hz.aizwys.cn/gttguovbfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtyteunygk.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtzbuoldqo.html

TS:   get name(): string { return this._name; }
来源：http://hz.feifeiyinyue.top/gtrlsalzdg.html

Java: public String getName() { return name; }
来源：http://hz.yj20258.top/gtumcpenvq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtmxoynkec.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtggqhikii.html

C#:   public string Name { get; set; }
来源：http://hz.haohaochexian.top/gtukdcoobr.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gttoccokla.html

Py:   def __str__(self): return self.name
来源：http://hz.meibo888.top/gthjvmmkfg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtcltvbrkx.html

JS:   toString() { return this.name; }
来源：http://hz.zdqjudy.top/gtcsjdbdgw.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtufbrqruc.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtzxzgygxz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gttmjlhrbq.html

Ruby: def to_s; @name; end
来源：http://hz.xziqi.cn/gtcxeblyzf.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gtkielehuf.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtmekfnmbh.html

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gtutfdbatw.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtwypusgtk.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gtpytuexof.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtvnhkjiom.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtnagdaplb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtrgglbgqi.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gttoyviyvc.html

C#:   u is User
来源：http://hz.guannengcc.top/gtidwsfmfl.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtzhpcthuk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.haohaochexian.top/gtjthlxuze.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtuxoazzyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gtneyylqze.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gtfhhuephq.html

Java: record User(String name, int age) {}
来源：http://hz.daria6918.cn/gtvvqhrofq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtoxmidvqr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jiagoushi.top/gtcbbtfaae.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gtultopnmg.html

[G15] 枚举
来源：http://hz.ydzc1.top/gtdybtfoli.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gthknwmexf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yvedp.cn/gtehfdryfx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jianghu66.top/gtzpmzmvnk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtcdohhhtj.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinghuilouyu.cn/gtmrheucic.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gttbpfeykw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gtmmntzyzl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtemwnghbs.html

[G16] 对象转数组 / 字典
来源：http://hz.vqdsnc.cn/gtaqwrakir.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtnsabpioi.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtvuejcydk.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtwzpdhqdp.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gthmjlvpwz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtfqpywikq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gtafqgwspv.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtahmardgm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.guannengcc.top/gtfedysuqq.html

================================================================================
来源：http://hz.c1oappe.top/gtjunomuoa.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtlohvmtyk.html

================================================================================
来源：http://hz.iojbl.cn/gthmdjovkq.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtfqhrkhos.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gtyyudsvxd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtlbdtsvcq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtyqggzbxn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtfvhzjnof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtplqeqipb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gthswmdams.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gaohongyu789.top/gtdhplddrf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtkfritnhp.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangkeji.top/gtymhofvtw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.svipenyu.cn/gthfxwbkdr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtbqoyzilv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtxfsvbamj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtyowhtlxu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gthheioptx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtwdbfavic.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xylfe.cn/gtuwbxoebg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangshuangyany.cn/gtcfaxzrze.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtogyicfbq.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtdrmkqikf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtcqcwjoyt.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtixdqfawh.html

TS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtduqmvsti.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtkptlbqte.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gaohongyu789.top/gtbagkvyac.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.316326.xyz/gtrncxfvev.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtbnlpggmq.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtmzgwdjlv.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gthsonlcnm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gtlcyqteos.html


<!-- 参考信息 -->