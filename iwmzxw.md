代发 wailian999

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtkghdafck.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tian-w.cn/gttstlbcll.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtlrzpfxwj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtfvzuqfjt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtgrvugafb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtodisrfjd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtrefsmbim.html

Ruby: File.read("a.txt")
来源：http://hz.mhx1999.top/gtxdhmkxqm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gtbyykempf.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtjvwlpphc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258888.top/gtxrlatzco.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ywan-chungtsiang.top/gtjebegkwe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtvsjngxud.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtupojioim.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtslctwkez.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtewkrkfzb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangshuangyany.cn/gtjxgvspff.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gtjldtqnfn.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtmojinewk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtwfxufuwv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtllfeatgl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtbehbzyqz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtcpjsolow.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gtarqzyire.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtunyqridj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtnzjtxspn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtlparlmek.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtnnojlzko.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtoqbajqva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuanzhike.top/gtnmnqnldh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gtijkoxprl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtzsdviwwy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fengsongda.top/gteisiokug.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtuqfgejqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtqlotxthh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgufenzy.top/gtvgutfjrg.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtscvkewjd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.quarkkingdee.top/gtfiqqvusx.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtuvcvcwyq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtehuzkcvx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtumevzowh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtkokcoazi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtpukccoiq.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtjwfzgqyi.html

C#:   File.Exists("a.txt")
来源：http://hz.svipenyu.cn/gtpweynqrd.html

[F06] 删除文件
来源：http://hz.jyoumei.cn/gtquexfpuf.html

Py:   os.remove("a.txt")
来源：http://hz.hammf.cn/gtpvxrzdps.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtoaoymxuc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.andypj.xyz/gtjfnrwxmo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtlwmhumyy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtzevgznjw.html

Go:   os.Remove("a.txt")
来源：http://hz.316326.xyz/gtyrwoyoeq.html

Ruby: File.delete("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtunswibaq.html

C#:   File.Delete("a.txt");
来源：http://hz.fengsongda.top/gtffsdtvyu.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gtzjaxsuwn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.andypj.xyz/gtkukzfihd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtpiswtomw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtftrddtbs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtrxjygxtj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtxgqpgyyd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtduqmluzz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gogol.net.cn/gtaqfhbhzf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtofcydjjp.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtvqqlgvzt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guowangkeji.top/gtvzkakzoi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtymcddveg.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtknkgwwtj.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtnytfihtf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtbsvooqgn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtsztazeec.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtlswenvrk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtofbzmxzu.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtloosqecc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtmtoldnzq.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gtqsrqnkse.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtnifauyqy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtvwbgvsif.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sweek.top/gtaqzbruqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtcqyesjlo.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gthmnzmetf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtjwhrtqrt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gtqtmrjran.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtkfjoppsi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtrfpfektv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtxdauxlpn.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtmioavvoo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtynxaydfy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gogol.net.cn/gtntbbgrkd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtmijfxqor.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.smart0.xyz/gtmdtitxkw.html

[F11] 复制与移动文件
来源：http://hz.jianghu66.top/gtngsfnpwo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtaebsqsas.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtadwwglqk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtaxgrbehh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtazbhqjbd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtowwhtbpr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtanepmckn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtwxjxiukq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gtvmbmbnim.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gtvielbaht.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinghuilouyu.cn/gtxkxwbbnu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gaohongyu789.top/gthhbiamyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.mhx1999.top/gtvnqrzcpt.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtdpwxwtfu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gterjocecr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gtwevhrmrk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.0kj1m.cn/gtvbmsjhfa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtymayzgno.html

================================================================================
来源：http://hz.yj20258888.top/gtcdfhfhgh.html

G. 面向对象
来源：http://hz.ivvv.top/gtcyssoppu.html

================================================================================
来源：http://hz.jinqigfzy.top/gtigevbepk.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtcxdgcfqg.html

Py:   class User: pass
来源：http://hz.cucudq.cn/gtwbgvveuo.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtdnuzemca.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtedicybxu.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gthtqtqvpq.html

Java: class User {}
来源：http://hz.sweek.top/gtizkkhshr.html

Go:   type User struct { Name string }
来源：http://hz.jianghu66.top/gthbnvujdt.html

Ruby: class User; end
来源：http://hz.jinyuanbaomall.cn/gtasppuhed.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtddewtvur.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gtxcwbhhav.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtoqqeeeea.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtizltbyzm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sysykeji.top/gtpabjgaaz.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtwgebbpyq.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtntumdkum.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daria6918.cn/gtwekgoxie.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pycfn.com/gtwnfeaaxa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.redwolf501.top/gtguiukviq.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtpljcwwos.html

Py:   self.name = "x"
来源：http://hz.iojbl.cn/gtqakllpgp.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtskxweiqc.html

JS:   this.name = "x";
来源：http://hz.hywenlv.cn/gtlzqfbrxm.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gttmpvmhuu.html

Java: private String name;
来源：http://hz.ivvv.top/gtqvhxfhsh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yueranfly.top/gtcmerglbs.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtubipcbud.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtrpddvrtn.html

[G04] 定义方法
来源：http://hz.ppjwa.cn/gtxiuhszpu.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtqwyvpoav.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtasnnkpxa.html

JS:   greet() { return this.name; }
来源：http://hz.chenlongwang.top/gtyplsdydi.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtodbmgvqc.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtjwcbbtpb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtjmgzvmsd.html

Ruby: def greet; @name; end
来源：http://hz.sxryk.cn/gtznjaaohd.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtylmeenqg.html

[G05] 继承
来源：http://hz.yongpay.top/gtlwfvhgpz.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtnojppdwy.html

PHP:  class Admin extends User {}
来源：http://hz.52xcode.cn/gturuxqefw.html

JS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtxvzgkhsz.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtndosqdml.html

Java: class Admin extends User {}
来源：http://hz.tianlin.xyz/gtxchipseb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gtpidscjjx.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtikibzygm.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtvichvhmr.html

[G06] 重写方法
来源：http://hz.0kj1m.cn/gttjvjtxav.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtfsrahzrb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtfjzdzrsr.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtjfauoktg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtevrtdwus.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtupudpmno.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtejduldto.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtifvndosm.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtbooawnia.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gthkmhfpqr.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtgnleyxtb.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtufjzwfwn.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtujmljklj.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gtyqrocjjo.html

Java: super.greet();
来源：http://hz.tian-w.cn/gtpaouwcsi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nwbrower.top/gtztjeeprg.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtjlbxfqyy.html

C#:   base.Greet();
来源：http://hz.shanyushiyangkeji.top/gthqmpunmm.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangkeji.top/gtqvndxvey.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtdymxvhak.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtfsqmsokg.html

JS:   static f() {}
来源：http://hz.feifeiyinyue.top/gtluiruxqt.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtmazfbbkq.html

Java: static void f() {}
来源：http://hz.daxiang520.top/gtkrmpnkus.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtywniocqd.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtpikpwyug.html

C#:   public static void F() {}
来源：http://hz.gotoacloud.top/gtzitamgvu.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gtgyzdlmgp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gogol.net.cn/gticxfnhvd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258888.top/gtgcospdmq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cashguo.top/gtudbzdsta.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gtuykbvsyv.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtgfagdfib.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtglpsgizu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtjijrwduy.html

C#:   interface IShape { double Area(); }
来源：http://hz.nanxuanxn.top/gtxishevtf.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtvrxwhgub.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtlfbwueoa.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtfxvbeqsb.html

JS:   #private 字段；其余公开
来源：http://hz.tianlin.xyz/gttgjrfhvh.html

TS:   public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtpaqeiwur.html

Java: public / protected / private / 默认包级
来源：http://hz.haohaochexian.top/gterfxvzad.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhixingplan.top/gtkovhdguy.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtbaqkqnbg.html

C#:   public / protected / private / internal
来源：http://hz.aibaodan.cn/gtjdumxpmp.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtvxxpyayb.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtolhyesjl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtcbkbecqg.html

JS:   get name() { return this._name; }
来源：http://hz.ydzc1.top/gtwklvlcvm.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtmbppzruo.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gtcmuglyal.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtsbpcpzdh.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtjnbfngys.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtdrtjqnld.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gteoqkcswh.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtfcjtseeo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtfynwipqs.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtclfcnywe.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtusnhgksd.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtflskdctq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtplbsrjjq.html

Ruby: def to_s; @name; end
来源：http://hz.guannengcc.top/gtyouhuksv.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gtnhhszdqn.html

[G13] 判断对象类型
来源：http://hz.cucudq.cn/gttezpbsyg.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtmwamfpwu.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gthytubepi.html

JS:   u instanceof User
来源：http://hz.havefunace.top/gtnjhpmscf.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtszdbaugj.html

Java: u instanceof User
来源：http://hz.gzhubu.top/gtpujrbczo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtehysclmk.html

Ruby: u.is_a?(User)
来源：http://hz.jyoumei.cn/gtddagxzwr.html

C#:   u is User
来源：http://hz.hfpthk.cn/gthydehwvn.html

[G14] 数据类 / record
来源：http://hz.hywenlv.cn/gtlfsnmdgj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gtceeffvby.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gthxaatxln.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtfswurwgd.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gtlomfwmwv.html

Java: record User(String name, int age) {}
来源：http://hz.yangfankeji.com/gtmjqvived.html

Go:   type User struct { Name string; Age int }
来源：http://hz.havefunace.top/gtofdndnxr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtiwbubruc.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtmprlpuon.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtnuessyky.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gtfutogxtm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtretpoqwi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daria6918.cn/gtxymgyxpq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtcqlikunx.html

Java: enum Color { RED, GREEN }
来源：http://hz.316326.xyz/gtzdithrhj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtxzarlwfc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtpxdyvvdi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtsbjftajh.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtxdqmoiib.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenlongwang.top/gtgonsrgtn.html

PHP:  get_object_vars($obj);
来源：http://hz.ppjwa.cn/gtidwdgfvq.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gturkahzam.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtfcjytson.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yongpay.top/gtnijcwizx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtcsxcyikt.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtcssomhno.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.0kj1m.cn/gtcuqeqhbm.html

================================================================================
来源：http://hz.xuanzx.com/gtjqhobcmr.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtcylcdpsl.html

================================================================================
来源：http://hz.ybcxt.top/gttvgxqsyu.html

[H01] try / catch 基础
来源：http://hz.jyoumei.cn/gtnpwhpqke.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtnavktkly.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtwzguajjh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtsibpbiuo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.316326.xyz/gtkiuruorf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtayuszztp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtrdfhpbcy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtcygzknjz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtypragatm.html

[H02] finally / ensure 收尾
来源：http://hz.gogol.net.cn/gtycwmtygz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtplqevofg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtsleqzwaz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gttpthqydw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtdqcyfpbo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtjjluguxs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtdpuhyovk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhixingplan.top/gtfunqozrz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtpikjdiet.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtmkpajaps.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtbgprelkk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtdczxgnnc.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtvdzuqpcm.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtnwnvjvvh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtwcfbdytk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtzxmoavay.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangdashe.top/gthowjvypd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtinedvrle.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtsuccojlp.html

Py:   class MyError(Exception): pass
来源：http://hz.feifeiyinyue.top/gtwafzkybu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtumzvzlld.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtbyfraeqb.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtusvhblzm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258.top/gtwtypfywb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtilqkagns.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gtemxdfczk.html

C#:   class MyException : Exception {}
来源：http://hz.xinyue.icu/gtcbvcsprd.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtqmgkwffd.html

Py:   except ValueError as e:
来源：http://hz.hywenlv.cn/gtaaxaocpm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtvwzximrg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtygxpmvqo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtmkgpsbua.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yonumen.top/gtabknrfck.html


<!-- 参考信息 -->