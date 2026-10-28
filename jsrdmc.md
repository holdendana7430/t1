代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.xylfe.cn/gtwottuxsa.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtipftyhpk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aibaodan.cn/gtjwxiesxx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtmnahticr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtvpeefygo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtrsnchzdl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtzzqxywix.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtlfowjkia.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenzaomai.com/gtofiqnmlm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtvoxrchqw.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtbgbrojww.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gticljqvct.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtjzzxgsux.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gturpzuqcg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtczxhoqsw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtbiekygdl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtdsfnkhca.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xinyue.icu/gtihxtaqxb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtzrwhgzxi.html

[F04] 追加写入文件
来源：http://hz.aizwys.cn/gtzcbdrztl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangdashe.top/gtfjibcllq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gttrgoibez.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtmvnokcpy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gthkqbjvmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtlmzzwlxq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aizwys.cn/gtkwgpohhx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zdqjudy.top/gtplspnbsk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtmkjlfdax.html

[F05] 判断文件或目录是否存在
来源：http://hz.jianghu66.top/gtjcwdmpdm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sxryk.cn/gtywgijoru.html

PHP:  file_exists("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtjpfgayas.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtrmbjywth.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtzzutcpyd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtdolxlhkd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgfzy.top/gtwobfnqzn.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuxming.cn/gtlbxgcpxp.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtwrdyfxux.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtgxpqgrrm.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtnjlktvwa.html

PHP:  unlink("a.txt");
来源：http://hz.jlsjyb.cn/gtvgoxzari.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtojgbfomj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtlpxeqint.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtvjkdhumm.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtvznpgqyu.html

Ruby: File.delete("a.txt")
来源：http://hz.smart0.xyz/gtvqaokghm.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtjmpfqfla.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtnoelxwqt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuxming.cn/gtizbwcdme.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangtech.top/gtrorurwet.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtsbzehlap.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtvckbozgp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenlongwang.top/gtamuhvxjr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daxiang520.top/gtinmyofaz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xinyue.icu/gtiagvkipg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtkmmxzzhw.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gtkixvikuh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtbccpsxki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtzigzpsbt.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtxveishxs.html

TS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtjgbqtwzn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tianlin.xyz/gtaufizqam.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gterlpendh.html

Ruby: Dir.children("dir")
来源：http://hz.havefunace.top/gtovkrkmli.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jianghu66.top/gttezgxmfk.html

[F09] 获取文件大小
来源：http://hz.havefunace.top/gtvxnwkodv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jlsjyb.cn/gtjuyedkbe.html

PHP:  filesize("a.txt");
来源：http://hz.jinyuanbaomall.cn/gthzrrslps.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtwypdflhb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtjaqihjqz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtmwtqealm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxinkj.top/gtpemoujzn.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtqjkukwos.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gtitmodisx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtaaiefnqo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtuajantlh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gtmsxgibdx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtaqsbgzni.html

TS:   path.extname("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxowkvxup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.c1oappe.top/gtkgumoegh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtjwxdnvps.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gttzngrqah.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yangfankeji.com/gtixiqiewj.html

[F11] 复制与移动文件
来源：http://hz.pycfn.com/gtztxrrcub.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtrgbmjsal.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtamzztibr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtelfstyuo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtcbqootpx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtehxxclpb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangshuangyany.cn/gtdtvndkjj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtshxdootk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgfzy.top/gtqwghkjoq.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gtqbrwpfze.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gttlwtsujt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtpaqkeqjv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtbhytswtc.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtdhgtdsdq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtmqafltir.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gtndbxlyro.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtlojkdwdv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtzkneyndb.html

================================================================================
来源：http://hz.yangfankeji.com/gthpyinlkf.html

G. 面向对象
来源：http://hz.hnqzz.top/gttzgufykx.html

================================================================================
来源：http://hz.smart0.xyz/gtjxmquehi.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gttfcukxha.html

Py:   class User: pass
来源：http://hz.quarkkingdee.top/gtbcvkmhkf.html

PHP:  class User {}
来源：http://hz.sweek.top/gtcfiogrpx.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtgtfpjnom.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtraerjogn.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtqcxdvptl.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtwfltlfoc.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtjxwnosxr.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtuqdmvqnv.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtcsrbhjxf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtopbcdbcg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guannengcc.top/gtkeuqctrv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gthbtwlavx.html

TS:   constructor(public name: string) {}
来源：http://hz.ybcxt.top/gtbmbsyxcm.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gtaigurknr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtyfswsqml.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hysaishi.cn/gttuzwmlhr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtsrxtthoy.html

[G03] 实例属性
来源：http://hz.gzhubu.top/gtoyikiaaa.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gtzqlmemjd.html

PHP:  public string $name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtggpoopcl.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtahqcsegh.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtjpbbsnsh.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gtypjnpvrg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtdktueyqj.html

Ruby: @name = "x"
来源：http://hz.zhijiandao.cn/gtzxlkavkn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pengpengdd.cyou/gtlqtlbamy.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtqopqlbyw.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtrzqjvqdl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtfyculjrc.html

JS:   greet() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtqcpvlsem.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtfalwnoho.html

Java: String greet() { return name; }
来源：http://hz.guannengcc.top/gtoxxwfesf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangdashe.top/gtnqulfkxg.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtjwyyvgio.html

C#:   public string Greet() => Name;
来源：http://hz.snrcjt.cn/gtcbbmmvah.html

[G05] 继承
来源：http://hz.jqgfzy.top/gtjdnumdgn.html

Py:   class Admin(User): pass
来源：http://hz.svipenyu.cn/gtnkfvqxkt.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtjarqapzz.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtmljgwsud.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtojmpages.html

Java: class Admin extends User {}
来源：http://hz.hywenlv.cn/gtnwuvcebz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtevhllpvv.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtpacghvin.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtzbthrssa.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtynlgceck.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtmxklrgoh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtasiqoump.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtwduraspz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtpcfroyay.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtcqormtup.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtlpowtqzb.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtvhuuoise.html

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtonbgrfaw.html

[G07] 调用父类方法
来源：http://hz.ydjk.org.cn/gtmizvxqkp.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gtvevqsyvu.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtxvwiajed.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtobgpwynq.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtvdveojbt.html

Java: super.greet();
来源：http://hz.cheryme.top/gtpjpdryag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtmybkjabv.html

Ruby: super
来源：http://hz.xylfe.cn/gtymklephb.html

C#:   base.Greet();
来源：http://hz.tanke756.top/gtvugpebzs.html

[G08] 静态方法与属性
来源：http://hz.yj20258.top/gtjnyfgtrd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtuxunrmft.html

PHP:  public static function f() {}
来源：http://hz.316326.xyz/gtvycglzpi.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gtqbyqgfpz.html

TS:   static f(): void {}
来源：http://hz.ppjwa.cn/gtkvpxdscd.html

Java: static void f() {}
来源：http://hz.sxryk.cn/gtsjlrdxrk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtrqxyhvui.html

Ruby: def self.f; end
来源：http://hz.andypj.xyz/gtlwegdqnn.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtvdgvryyg.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtpqmpedzq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.quarkkingdee.top/gthywqonvl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtcbaooxuc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jyoumei.cn/gtrcitwuit.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtmhdkcerj.html

Java: interface Shape { double area(); }
来源：http://hz.yangfankeji.com/gtcietuecz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jyoumei.cn/gtclgpizud.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtmdfqowbi.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtzmaodcie.html

[G10] 访问控制
来源：http://hz.tianlin.xyz/gtafiuzdnb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.smart0.xyz/gtfynvthgq.html

PHP:  public / protected / private
来源：http://hz.zhiwuduotai.top/gtnupbvdkh.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtkrorveoo.html

TS:   public / protected / private
来源：http://hz.hongshengwenyu.top/gtbisrdart.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gtnshwojre.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtmteaznsm.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtgrvcpyxx.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtgdxmravq.html

[G11] getter / setter
来源：http://hz.9152youxi.cn/gtezirhtje.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gthqqyylob.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtlrqbiaex.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtoqziwnfh.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtnvsfgcyy.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gtmfyckpuy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtnbsbrfnf.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtezifhfwr.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtfzziikct.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtozqvolgg.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtwvtgzckc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtjhidotof.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtuwtxmtyc.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtvovnjvcz.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtckdricmc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtadldcutt.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtqamcnonb.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gtzqjaweov.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtaiiegrbt.html

Py:   isinstance(u, User)
来源：http://hz.aibaodan.cn/gtfihqtdif.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtrgyjwhfn.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtyyfncekl.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtbbrgksqa.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gthvptnpll.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtlidiqvbs.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtpzaumxlw.html

C#:   u is User
来源：http://hz.feifeiyinyue.top/gtnjdnhabv.html

[G14] 数据类 / record
来源：http://hz.shangyingyoupin.top/gtuwtihioh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtwcywkzwr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtmgewhyve.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.bjfxy.top/gtlnkauzsr.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtrdmlbgma.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtdkhvtalv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258.top/gtqziussmo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fengsongda.top/gtazsyiwmc.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtbhsdooeh.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtvudydghf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gttogsscet.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtrbuwfqng.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtdfxxetzn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtijjasbzv.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtiwvafrmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtbkedqvuj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtzsnkjtaq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtsdefusip.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtqyyxutwy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtywuvamms.html

PHP:  get_object_vars($obj);
来源：http://hz.gogol.net.cn/gtarvclssy.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtzzromydd.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtjurtnyux.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtobtcxvja.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gtacbnawky.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gteruotxix.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.kuanghao11.cn/gtzeffqcfw.html

================================================================================
来源：http://hz.ydzc1.top/gtkgoucfzs.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtxtxfqfaj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfhjtanoh.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gtfhtsqaek.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtgxcqzecs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtjyoynjjf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtsyiqbvyd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtgtnniqjm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtemwflkmg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.c1oappe.top/gtxkaquhzi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtmodvjotr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtbaecqbns.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gtvkzyiwua.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gthvbiypbw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtzxmmvrdw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtlaucddrc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtnvlankgj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtbthzbinb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtpldwiaje.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtxgyopxdg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258888.top/gtfhygoxhu.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtfznkqnpu.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxinkj.top/gtuoygvqye.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gttomkbkxu.html

JS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gttfybdhvg.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtppbtkmng.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtnfwdjekr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtrwbqmgfm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtlrfnlfgp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtgppyxiow.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtwjznzcbn.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gthtbhpdhq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtslmgknrn.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtyrdywcls.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtqyjkdzsx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtwqyacrur.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gtlkanhwhx.html

Ruby: class MyError < StandardError; end
来源：http://hz.cdnleiting.top/gtbvklqxyb.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtnenylcqj.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gthstsvzxb.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtbfgvchro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gtsaoqqxgi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gthspacxkx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtszbithyv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtaljpdxyn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gthcayabfe.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtnlnoofez.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhoulong.xyz/gtkxpiaoht.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtdnpzclec.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtypgddmli.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hammf.cn/gtuuyntkob.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtrqkgghrm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gthzwuwvgr.html


<!-- 参考信息 -->