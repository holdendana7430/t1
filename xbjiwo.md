代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtdvmifijt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aibaodan.cn/gttmrmhjim.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sufxvd.cn/gtplasqnoh.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gttajoftti.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtourrbcie.html

================================================================================
来源：http://hz.yvedp.cn/gtvqnswzph.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtvdsjrxca.html

================================================================================
来源：http://hz.meibo888.top/gtkczbndqu.html

[F01] 读取整个文件
来源：http://hz.hfpthk.cn/gtetowasmj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtrttzgtvl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cheryme.top/gtyewckukq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.haohaochexian.top/gtcwdnthgd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gtaogqogmh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gthycgssqm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.c1oappe.top/gtzvfhsmfx.html

Ruby: File.read("a.txt")
来源：http://hz.zhongyouzk.top/gtuksfjvrz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yongpay.top/gtjvjvvxyh.html

[F02] 逐行读取文件
来源：http://hz.yj20258.top/gtarfgieel.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtbfazswix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhengqikj.top/gtopxrumuc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtzmegbjer.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gttvstaorq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtccahlczh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gtnpmssphr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtfdksdhok.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenjidiqi.icu/gtnzxtkydk.html

[F03] 写入文件（覆盖）
来源：http://hz.svipenyu.cn/gtbblcjzxp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pengpengdd.cyou/gtaiuoizfp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xziqi.cn/gtgzchoqaz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtqhdxzjnd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtghxtofnt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.birdmap.top/gtedjvgtfv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuanzx.com/gtqzrjmnpr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtqudgszrb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtvejsyspe.html

[F04] 追加写入文件
来源：http://hz.sysykeji.top/gtwiamftjk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgfzy.top/gtodinibyb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangdashe.top/gtiejjxgxi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtmnbpmrkm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtqtrdbveq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtoezjzkyd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangdashe.top/gtojkkrmzm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinghuilouyu.cn/gtacnskofx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhiwuduotai.top/gtcqvnskxp.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydzc1.top/gtebgbmyzp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtwvynpzca.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtquwvuomg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtvszbqcjg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtscfnfbws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtpqykopxo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtiodzpijt.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtwsfhmstd.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtzubntnzo.html

[F06] 删除文件
来源：http://hz.feifeiyinyue.top/gtbzxtcsaf.html

Py:   os.remove("a.txt")
来源：http://hz.yuxming.cn/gtlfxlzkei.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtmdzoxelu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gthoftbrti.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtmldzebmp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtbjmaojkz.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtxsfrmpzq.html

Ruby: File.delete("a.txt")
来源：http://hz.zhiwuduotai.top/gtercclrrv.html

C#:   File.Delete("a.txt");
来源：http://hz.ydzc1.top/gtecjzkput.html

[F07] 创建目录（含多级）
来源：http://hz.wangshuangyany.cn/gtkstwatge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hysaishi.cn/gtqqzemibu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuxming.cn/gtmvvisqts.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtokmqyfzm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtalztnkea.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gtexxbhqba.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pengpengdd.cyou/gtkayxylnr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gtmzgsudit.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.bjfxy.top/gtcxwpihzy.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtercqcxma.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtjvtywamo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtwzijhmdy.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtyyrlkufv.html

TS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtshbouknm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtvbmkiqig.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gthlatlvlc.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtroadwuuf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtzxicrfzq.html

[F09] 获取文件大小
来源：http://hz.iojbl.cn/gttsxkbjxl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xylfe.cn/gtijwznbcu.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtxlirmvnz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtnehficke.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gthxbdhyfc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtzeqdkwlv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gthohmcjgb.html

Ruby: File.size("a.txt")
来源：http://hz.chenlongwang.top/gthnnirbec.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtvmglkkcy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtqnlhygww.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtplpmyrem.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shzxlz.cn/gtdfbzouie.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtcggbpbae.html

TS:   path.extname("a.txt")
来源：http://hz.yonumen.top/gtsgehrjrb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydjk.org.cn/gtnnbfeaje.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtqwywgags.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtuegfjgcd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtpexaeecc.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtoctctoxr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtupsfdwkv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtpftqchzt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtfizzxiei.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtugcqzepc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtodkwnfit.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tanke756.top/gtwuzeehzz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtyndyaeei.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gtqkrnmzap.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtamhlhryj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guannengcc.top/gtnsuspxtr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gtumumjjpq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guowangkeji.top/gtoyesoeea.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtcpukytsg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtisglvkyo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtsqypwizh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gtkoligprj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hywenlv.cn/gtmokeuyld.html

================================================================================
来源：http://hz.zhoulong.xyz/gttqkkmrur.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtqoniqvyy.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtohucmhjz.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gtawnqflcz.html

Py:   class User: pass
来源：http://hz.chenzaomai.com/gtlksmyiei.html

PHP:  class User {}
来源：http://hz.shzxlz.cn/gtvycmbiko.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtmfrtljec.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtlxwoxtqr.html

Java: class User {}
来源：http://hz.hongshengwenyu.top/gttxjjwvgj.html

Go:   type User struct { Name string }
来源：http://hz.meibo888.top/gtbrmkjeet.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gtspbiqvfe.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gteiszhupq.html

[G02] 构造函数
来源：http://hz.meibo888.top/gthekcoflz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gttvpfilrh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtouzgzjap.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtaugnbryy.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtuhvsizfl.html

Java: User(String name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtvzckfyev.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gaohongyu789.top/gtlpqlwnid.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtgtajauoa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gthomhwaui.html

[G03] 实例属性
来源：http://hz.cheryme.top/gtbylwfvjo.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtzywfqsry.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtmmrodkqc.html

JS:   this.name = "x";
来源：http://hz.zhongyouzk.top/gthevibwfp.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtrwebykgl.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtmdesjtvu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuanzx.com/gteanngruf.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gtsdolfluq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtditvlbxz.html

[G04] 定义方法
来源：http://hz.jianghu66.top/gtockptkir.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtkcrfofqq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtcltftbcg.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtwlsazwvc.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtknkbdfmh.html

Java: String greet() { return name; }
来源：http://hz.ivvv.top/gthsyponvd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtueamvbgv.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtivivsrli.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtqpgwfulv.html

[G05] 继承
来源：http://hz.kuanghao11.cn/gtndbfrvml.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtkuxqqhgc.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gtrigknorr.html

JS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtbvkhccnk.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtljvrvbzj.html

Java: class Admin extends User {}
来源：http://hz.chenlongwang.top/gtgfhgupld.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daxiang520.top/gtswxjxkhs.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtlkjeqdse.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtyglskdsw.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtkxzmnldj.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtereinhrc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtcmhgdrwk.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtqqnoiufd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtfpjylgjj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtifmhfrbu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtpfunuumu.html

Ruby: def greet; "admin"; end
来源：http://hz.cheryme.top/gtbbnzcxpq.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtqzkuuguv.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtzmwrewin.html

Py:   super().greet()
来源：http://hz.quarkkingdee.top/gtbpqyfuvc.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangtech.top/gtmbmbljyu.html

JS:   super.greet();
来源：http://hz.chenzaomai.com/gtycfrjwyb.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtcrnslcea.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gtckoxkytf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtmrvwdqem.html

Ruby: super
来源：http://hz.chenzaomai.com/gtmezjlzlw.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtohcsxkxc.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gtyfiqrdet.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gthekqhbfw.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtckbvdhvx.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtvkxninby.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtbxulbccu.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtbtudavzp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gtvgiwrfty.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtpvtupztl.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtptlkwvin.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtjgwyqsfc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtnqsjnopj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jiagoushi.top/gtorpumweh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xziqi.cn/gttxiwinpo.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtxwouqdgh.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtfcmeqfhw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ywan-chungtsiang.top/gtduntbdki.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinyuanbaomall.cn/gtqhhdtkqj.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhaomingkeji.xyz/gtnuaalvsb.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtwhzpkhuf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtzboznxlp.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtqvrfepky.html

JS:   #private 字段；其余公开
来源：http://hz.kuanghao11.cn/gtrugkzhkx.html

TS:   public / protected / private
来源：http://hz.tanke756.top/gttxltiywe.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangtech.top/gtgzbxtieu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtwhquwjmh.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtrfadmndh.html

C#:   public / protected / private / internal
来源：http://hz.yongpay.top/gtuqdgorpz.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtnkcnegwb.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gtpnuvziug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gttvumtmuj.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtbktowvke.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtffemnktd.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gtwtmomxui.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yueranfly.top/gtrcncsoxl.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtxzngslxm.html

C#:   public string Name { get; set; }
来源：http://hz.hfpthk.cn/gtvqszutss.html

[G12] 对象转字符串
来源：http://hz.zhiwuduotai.top/gtvdsaidej.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtwrmerlan.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtpykffbwr.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtjyaqjnuj.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gtlcchohgk.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtjsydhxna.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtspyljazi.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtkcmrczad.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gthibucmxs.html

[G13] 判断对象类型
来源：http://hz.yonumen.top/gtsxtxqibc.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtqtngcniw.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtzosqxbuk.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtuydeksti.html

TS:   u instanceof User
来源：http://hz.jqgufenzy.top/gthlajwuae.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtdvkggtyu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gttfrlfvij.html

Ruby: u.is_a?(User)
来源：http://hz.mhx1999.top/gttnwafyoo.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtwcwemvuf.html

[G14] 数据类 / record
来源：http://hz.xingfuxueyuan.xyz/gtlegbswcj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtrhttyplg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtqwddntls.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sufxvd.cn/gtslmmaaou.html

TS:   type User = { name: string; age: number };
来源：http://hz.pengpengdd.cyou/gtpavgofik.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtvvzbnbvy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gtwggrmqmy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtrkizweph.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtdvjeaxfu.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtiztaxifk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtprnlcmcd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtsdqpdbdy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtafgffavm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtxvmxpdno.html

Java: enum Color { RED, GREEN }
来源：http://hz.svipenyu.cn/gtbklbvenc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangshuangyany.cn/gtvitstmvx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gttinbyxok.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtzlsphivf.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gthfjgygpo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtldqrewmb.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtjmwwsdzi.html

JS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtvlvtjbzs.html

TS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtlkpbicmr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenjidiqi.icu/gtlesuizwc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jianghu66.top/gtgpptnvfo.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gtqkgezwhz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtbxzktgep.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrgxkcltt.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtcpuqywan.html

================================================================================
来源：http://hz.hnxiangtu.top/gtekpvipxy.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtfjuyatlm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtqyfcpvre.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gtdpqcjlzr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtvshidhsy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtrueqlkhv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtrxsxotjj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtfekrrbtj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtvgrbwylw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtsopldliu.html

[H02] finally / ensure 收尾
来源：http://hz.c1oappe.top/gtcccijkpc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hywenlv.cn/gtabqdiwof.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtssssedal.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtnhcwflyq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtdjskgxut.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtvexfvfyc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtpkcknaxb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtxfohasuu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangshuangyany.cn/gtygpwlsrm.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gtiywzihit.html

Py:   raise ValueError("错误信息")
来源：http://hz.gotoacloud.top/gthsgekewg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtoplkujcd.html

JS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtnevqemwc.html

TS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtizazfjdz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gttdgvmzjk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gterwbuhwl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gtwpvctdgt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtntnunsvx.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtjgyvigza.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gtcmnhgprf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtquptrmus.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtxssamuat.html

TS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtbxdlwxga.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gttgcgydoe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtvmzkhugl.html


<!-- 参考信息 -->