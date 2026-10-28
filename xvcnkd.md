代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtjwwqzgpu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gthmeksvjv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gteyvnkwhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtotdvnkvh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtasktdugv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258888.top/gtydjaghpa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtagfccrxi.html

Ruby: s.bytesize;  s.length
来源：http://hz.mhx1999.top/gtorluexvz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtdvbzpdic.html

================================================================================
来源：http://hz.iojbl.cn/gtjzuooihg.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtdblicmiq.html

================================================================================
来源：http://hz.ybcxt.top/gtwdrryazb.html

[F01] 读取整个文件
来源：http://hz.xuanzx.com/gtaymgzaoa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtndtzwukr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ybcxt.top/gtwfaxbhza.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtwlhzxwiy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangdashe.top/gtdylkfnsy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtambxjhgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gtwygupvvv.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtejwdrtwb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigfzy.top/gtokqlwkwa.html

[F02] 逐行读取文件
来源：http://hz.xuetiantiany.cn/gtsfohzfdj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sysykeji.top/gtghgzoovu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258.top/gtcenqbwvc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtixlfnpkh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtkgjltcez.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gttuxxmavu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dianchejie.cn/gtshtwaqux.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxuanxn.top/gtltfzzurm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtmehcjwjn.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtdrhbwwjs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.haohaochexian.top/gtqudnvfxs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtjluwybqr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtfbvzefuz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gtfigtojeo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtnwmrmpyo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gtmlqmzaxy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.9152youxi.cn/gtlnxixnlg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtjvwzptjk.html

[F04] 追加写入文件
来源：http://hz.cqqwz.cn/gtfxwspazs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sxryk.cn/gtlwsqcpsp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258.top/gtlcrkzlgy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtbsmenorh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtmhxsyhql.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgufenzy.top/gtvtbpbuoc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangtech.top/gtuvdjtbnu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtyisywubw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.daria6918.cn/gtfjumdbsk.html

[F05] 判断文件或目录是否存在
来源：http://hz.haohaochexian.top/gtsphipwdz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yonumen.top/gtbgjawojs.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtopgvtmmh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtdjzcyuok.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtnqwpdgnk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtofzwdtmh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gttsosiiuz.html

Ruby: File.exist?("a.txt")
来源：http://hz.ybcxt.top/gtfzmjyjxt.html

C#:   File.Exists("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtltebxras.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtlxoosqzp.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtrnxnxnfv.html

PHP:  unlink("a.txt");
来源：http://hz.quarkkingdee.top/gtecrqjifj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtxsndyhww.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtjjeebsqw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gthrsasjoh.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtrhzgfmdl.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtxoevgvkh.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtpliybhda.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtzhvuyudh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtplzxkwsf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.c1oappe.top/gtflnnmqke.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtiuynndgc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtelsnqrle.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtmrokwmpa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yangfankeji.com/gtcuecrxcb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cdnleiting.top/gtgekokszn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtadzxwpcj.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtydnpkkth.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtnyipwbkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xziqi.cn/gtfosaonms.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtifvkulai.html

TS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtnnirqsmh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtzlljhmet.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtuyubvbbg.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtxgfglucz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtqestpiyd.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtbqhvnpzy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gtanzemvvp.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtxivuuskn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gthfuxqvoo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtinwprqyh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gttpwghbfn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtzrhdndyt.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtmxkfjbpi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ywan-chungtsiang.top/gtuuhymcip.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtabiqaxbs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtnmwaobzl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtjdbjporp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtwagvpaeo.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gtqdwkvlbp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yvedp.cn/gtwksgnrwa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxinkj.top/gtnwyssomo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtkovsuekm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtfoqkfyfh.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gtxfvjmgyz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtgpzencag.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.c1oappe.top/gtrijfmuhd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtnyeqxaze.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtxpeshktr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtzzizpwah.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtlbqexjcg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtvkcdgtku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jianghu66.top/gtazweaemh.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gttqzlwhzq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cheryme.top/gtqkuthtnc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtasdketyj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jianghu66.top/gtjyxgzyla.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtakpzibyq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtmcmyzytk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnxiangtu.top/gtmaoaocga.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtsmxjsovl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtypcqrrvy.html

================================================================================
来源：http://hz.yangfankeji.com/gtzflgqncs.html

G. 面向对象
来源：http://hz.fzhhl.top/gtuavdcxhz.html

================================================================================
来源：http://hz.sweek.top/gtovalbldo.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtpvkswitb.html

Py:   class User: pass
来源：http://hz.pycfn.com/gtyvobxoea.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gttrngrucy.html

JS:   class User {}
来源：http://hz.yangfankeji.com/gtsxcmjtze.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtywvheqhz.html

Java: class User {}
来源：http://hz.meibo888.top/gtoiceqxfb.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gtxvcbjqhg.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtskjtwzux.html

C#:   class User {}
来源：http://hz.yuxming.cn/gturiizlsp.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtxuunzhaz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtznnhetng.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtdorztpge.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtgshrelhp.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gtobchqiov.html

Java: User(String name) { this.name = name; }
来源：http://hz.gzhubu.top/gtticutzmq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtggvsbfxn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtgujaueif.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangkeji.top/gtpgwisnwd.html

[G03] 实例属性
来源：http://hz.ydzc1.top/gtcnoowrua.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtfeqidrnx.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtusmfjxsp.html

JS:   this.name = "x";
来源：http://hz.redwolf501.top/gtezvuyyus.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtdkgmfoqq.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtnjfyikwc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gtbabbxurz.html

Ruby: @name = "x"
来源：http://hz.jyoumei.cn/gtnajawqim.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gtzbyvloft.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtrnqutvhh.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gtvfxwrtmt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtjylybikz.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtcvmjjpcl.html

TS:   greet(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtnlpvnxxj.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtlaamkbsx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtjqkzopfc.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtjtumooff.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtyqeuduhv.html

[G05] 继承
来源：http://hz.yvedp.cn/gtnldaniaq.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtjkhrrdxg.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gthptwyata.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtqgigliiy.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtrozcsxjn.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtpdxkuoww.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.bjfxy.top/gtzanebsmm.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gtvnynzhux.html

C#:   class Admin : User {}
来源：http://hz.zdqjudy.top/gtjorxrnqu.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gtbolnphoi.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtlxtwfbap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtedujfvjy.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtsmibvnod.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtpqgveqev.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.smart0.xyz/gthmeskxwn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtfvhcelkj.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gtreoivaqg.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhongyouzk.top/gtxurqtaec.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtyiirwzfv.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtqudfqbkw.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangtech.top/gtubgpedjx.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtlbdyuive.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtmyxrimaq.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtlutdaytt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xingfuxueyuan.xyz/gtjibfgtsw.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtwddpdxca.html

C#:   base.Greet();
来源：http://hz.jinqigufen.top/gtcgoodhqy.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gttlyspyzk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.havefunace.top/gtztktlyet.html

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gtqcrdqicm.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gtynuxcldr.html

TS:   static f(): void {}
来源：http://hz.xuetiantiany.cn/gtsbmuykqq.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtejidgmws.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtlkrhidaq.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtleyemywn.html

C#:   public static void F() {}
来源：http://hz.cdnleiting.top/gtyvplmwew.html

[G09] 接口 / 抽象类
来源：http://hz.gaohongyu789.top/gtocyltotf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yongpay.top/gtsabkrnvo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtuikwoklc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtmjktriem.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtdtplhkuo.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gthvbfbydt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtixrkiars.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pengpengdd.cyou/gttrknqfes.html

C#:   interface IShape { double Area(); }
来源：http://hz.kuanghao11.cn/gtepvskkyb.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtkgyqyzue.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtanzbenyi.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gtwmtyvraj.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtpcbjfnrh.html

TS:   public / protected / private
来源：http://hz.dashuyun.cn/gtcnsaxxea.html

Java: public / protected / private / 默认包级
来源：http://hz.cucudq.cn/gtlmorwius.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtnbjnefiy.html

Ruby: public / protected / private
来源：http://hz.guowangkeji.top/gtywnhopti.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtocegyuuf.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtldqzgbqh.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtsbokkxss.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtlfogtzdz.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtkvcucjxr.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtamfzwxqz.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gtgkzzjybd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtobipdbwm.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtvvckemcy.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtwjdvrcnx.html

[G12] 对象转字符串
来源：http://hz.nwbrower.top/gtuqzdzjno.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gtixroxosb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtegckjzxv.html

JS:   toString() { return this.name; }
来源：http://hz.chenlongwang.top/gtgdxriwvp.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtgicxrlei.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gtdrtkwqpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gtcwmluqxj.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtymvkbasq.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gtqrmwhgyu.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtatuuyedt.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtzljiqbob.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtjhwkguln.html

JS:   u instanceof User
来源：http://hz.c1oappe.top/gtjbpitefa.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtbtloexlm.html

Java: u instanceof User
来源：http://hz.jinqigufen.top/gtzoolbidv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtdfnoraiq.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtjmuxankl.html

C#:   u is User
来源：http://hz.cdnleiting.top/gtyibovkms.html

[G14] 数据类 / record
来源：http://hz.zhiwuduotai.top/gtmroaqwmc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtkpuwflcz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cheryme.top/gtgxzptqpg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gthbfktccz.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtfuqaeaei.html

Java: record User(String name, int age) {}
来源：http://hz.hfpthk.cn/gtvukpqwxc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xylfe.cn/gtjdgdphcc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtrberyabq.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtlfziqjas.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtyegwjkom.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtyjvavzxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tianlin.xyz/gtokyrelyh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtcboubwut.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtvtsijqgp.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtgfwiwzsa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hongshengwenyu.top/gtdtvlssfr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hywenlv.cn/gtnlccberx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtckcrmgow.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gtqezupbcm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gtpdammzla.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gttpalsgta.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtqillqfai.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtcmhemqtv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sysykeji.top/gtiagidbjv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gthebixdjs.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtdzkkrdgx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtzoasyngp.html

================================================================================
来源：http://hz.zhoulong.xyz/gthdqhaxnc.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gteapvbhyv.html

================================================================================
来源：http://hz.tanke756.top/gtjbmooyam.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtvcldwbyq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gtewkebvht.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtilnxurbu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guannengcc.top/gtpoststox.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtklghxxgy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhixingplan.top/gtiletehjq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtfyvmslph.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gtblkxqxex.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtrqnrrbko.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtcnuzzxys.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gtezjdqxch.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gttdmftclx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gturbdanve.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtvxcywcng.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtstkehkdp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.9152youxi.cn/gtwrystcvj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtcynrxhzf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtllziviar.html

[H03] 主动抛出异常
来源：http://hz.yongpay.top/gteirtzbli.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtvapvdnqb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gthjzxoyoy.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtsadinmgy.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtwvcnlnhe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtduqqiwiy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtommdxqyi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtcxunvere.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtyxfthvpl.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtkodgjhrv.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtbnoobhsc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtaxsudrqm.html


<!-- 参考信息 -->