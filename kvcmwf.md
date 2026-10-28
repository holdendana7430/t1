代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtcikbzfzt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tanke756.top/gtlzmjfzep.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtpbjcjdqm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtajgrnqky.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxuanxn.top/gtrdrkxqjk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gttpdkxlle.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtlufqkpdv.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuanzx.com/gtlagcujcg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gtvhhkqxyh.html

================================================================================
来源：http://hz.xuanzx.com/gtimcpfszp.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtfwxnfgnx.html

================================================================================
来源：http://hz.316326.xyz/gtcuqbywnn.html

[F01] 读取整个文件
来源：http://hz.yuanzhike.top/gtzfgydwtt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuanzx.com/gtgtbkvkgn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gthsdgbnhk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtzrqlfhzb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cucudq.cn/gtczbkispq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtiywwqbma.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtuxxunfqz.html

Ruby: File.read("a.txt")
来源：http://hz.jyoumei.cn/gtxxalaxjv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sxryk.cn/gtubtgumcg.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtzblyaygx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtqjhvrxcf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gtyguhurop.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtjejutwlm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtbqhdmkak.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtbcscqvyv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigfzy.top/gtsxwbdyra.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtfebgjfnx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtvxxjmqmz.html

[F03] 写入文件（覆盖）
来源：http://hz.yanxiufei.cn/gtyekconaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtjkhecvop.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xinyue.icu/gtysxbgkmj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtbyeanamh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtouatfwtp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.redwolf501.top/gtglduczye.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtydhqiefi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtfzkdefxc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yueranfly.top/gtvzctwogl.html

[F04] 追加写入文件
来源：http://hz.fengsongda.top/gtfmrrzufz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.mhx1999.top/gtqtuiaodu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtxwqbezgu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtkdlailmd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtviwjkpfs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtnwmgzesh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.haohaochexian.top/gtfmxeafva.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtccuikqew.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shzxlz.cn/gtgycuogzk.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gttybihmgj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtyvfjcvjj.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtttovuadq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gtokaythms.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtnpenkvlu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtstewawuo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtrwhyaypo.html

Ruby: File.exist?("a.txt")
来源：http://hz.sxryk.cn/gtakrniyiz.html

C#:   File.Exists("a.txt")
来源：http://hz.guannengcc.top/gtniuxzqjg.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtbojvgjuj.html

Py:   os.remove("a.txt")
来源：http://hz.hnqzz.top/gtoezdnkwg.html

PHP:  unlink("a.txt");
来源：http://hz.sweek.top/gthbmprtjw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtnztkunpn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtjuwukglt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtqvsxwjsm.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtmhtdqzzi.html

Ruby: File.delete("a.txt")
来源：http://hz.yanxiufei.cn/gtlvhrajqt.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtnydyllwa.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtobydyhmf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gtpcvconrl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gteazmjcdf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gttnxfwhmw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtjcctgjtw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtscwlvxll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtsskocvfm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtxxrvutta.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fzhhl.top/gtsubyryse.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtbmwxoyvs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtwcbvulxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtovzpzqjb.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtsqrrwxcr.html

TS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtmofznjdz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtqxakcicb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtjqzqtddx.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtvojvkzzb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtxjvjgoih.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtrbbpeipf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtskrrkvvy.html

PHP:  filesize("a.txt");
来源：http://hz.sysykeji.top/gtwfjgnrwa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gtcgdwyrsq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtzltrfspp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtjooslthh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zdqjudy.top/gtghwdxcrj.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtsvvhbysq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shangyingyoupin.top/gtnklfjgqb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtekgbhkgi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtdkxekdrw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtokbyjghq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtlyborhjy.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtspmbohxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gtqmaugkwp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtgrxtsajc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtjzgvlipe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtgmrxqmia.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gtuqvtjgul.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtiharlwtz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtlzeadgip.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtlghsjbfj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtrxqummqj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtaetwzicj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtkopllccw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gtmpshbpnp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtojqayith.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gtxtgkiuqn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtpuvbxejb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.svipenyu.cn/gtocceeukq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtctiyljkk.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtraganrna.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtcxvadxkz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtwnwdaroo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtptcduzpt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtxuhrtmbl.html

================================================================================
来源：http://hz.shzxlz.cn/gtlweopcmw.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gthifadrez.html

================================================================================
来源：http://hz.cucudq.cn/gtmywwxhuw.html

[G01] 定义类
来源：http://hz.hongshengwenyu.top/gtftjueyct.html

Py:   class User: pass
来源：http://hz.yuxming.cn/gtyibkzmtt.html

PHP:  class User {}
来源：http://hz.fengsongda.top/gtyejnxsea.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtvamimqdc.html

TS:   class User { name: string = ""; }
来源：http://hz.quarkkingdee.top/gtjrtjidgj.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtqeqtqwgf.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtyzquqgmm.html

Ruby: class User; end
来源：http://hz.shuidangran.top/gtxqfkquai.html

C#:   class User {}
来源：http://hz.hnxiangtu.top/gttoycsatt.html

[G02] 构造函数
来源：http://hz.zhoulong.xyz/gtdvblrrci.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.meibo888.top/gtfomwlswg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gotoacloud.top/gtcryhterh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtbcuauwgd.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtfrowsypv.html

Java: User(String name) { this.name = name; }
来源：http://hz.c1oappe.top/gtfqjrztaw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dianchejie.cn/gtsnikhnzw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jiagoushi.top/gtjvhldpfg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jlsjyb.cn/gtbgfddvpd.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtjiveacwz.html

Py:   self.name = "x"
来源：http://hz.chenlongwang.top/gtmvbotwtm.html

PHP:  public string $name = "x";
来源：http://hz.gogol.net.cn/gtzkwdunxl.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtlddqkcec.html

TS:   name: string = "x";
来源：http://hz.meibo888.top/gtmnwndewk.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtspsevcuu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yangfankeji.com/gtkwpxdckx.html

Ruby: @name = "x"
来源：http://hz.gotoacloud.top/gttjfspcao.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtrbcoomzy.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtiastgbaj.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtnmhicikz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtsnxtnqfe.html

JS:   greet() { return this.name; }
来源：http://hz.chenlongwang.top/gtqnsxbfkm.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtvfmeduxo.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtuslqepmw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.snrcjt.cn/gtnbgvdoiy.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtbhxvaxxg.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gthrzqfzoo.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtgehnokcv.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtomvscvlz.html

PHP:  class Admin extends User {}
来源：http://hz.sufxvd.cn/gtflgurtbz.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtonthwyxl.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtfurdprgt.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtuuqawrkc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gtxowqkomz.html

Ruby: class Admin < User; end
来源：http://hz.ehwqpu.com/gtezdyyjuz.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtrzvxzpcp.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtamqruise.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtufkgckgr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtmdtkdttu.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtikvimuvz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtlbmdenki.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtpgvhwidg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtjkkizsou.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtjvmeyjzj.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtdahaxoee.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtkvukwdgc.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gtcoqnfmba.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtrxomghdb.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gtblmhmlbz.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtbjfgjqnd.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gtctwqbmas.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtsmcvucgl.html

Ruby: super
来源：http://hz.jyoumei.cn/gtkamizkcv.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gthizlqpmn.html

[G08] 静态方法与属性
来源：http://hz.iojbl.cn/gtrtwiudgb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtqxmjfoed.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtpwzoznwu.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gttrpmcqwr.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtpfkvmoon.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtmovurxxl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhoulong.xyz/gtiisukzsk.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtbdwkeavi.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtqhanjhmn.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtlzrrayjk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtetiqswsa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtxzhmchnd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gtaffdjxlc.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangshuangyany.cn/gtoawymfov.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtqkepwenv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtizxxkqzu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xylfe.cn/gtuuykondl.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangkeji.top/gtbfhfylff.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gthkuywatu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtbzmbfswl.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gttgxtglxx.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtxpgjatuz.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtzojhvtah.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtuyamuyrn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gtjujcggyp.html

Ruby: public / protected / private
来源：http://hz.jlsjyb.cn/gtqumnfvdn.html

C#:   public / protected / private / internal
来源：http://hz.ppjwa.cn/gtmjzsytos.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gthxoaqxer.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtiiyxbuac.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtfmngioja.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtsmojneax.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxinkj.top/gtkjhnxtgj.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtxxrqtsig.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtnugnillf.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtchxaadsz.html

C#:   public string Name { get; set; }
来源：http://hz.jinghuilouyu.cn/gtmpglhmxh.html

[G12] 对象转字符串
来源：http://hz.cucudq.cn/gtptlfjwdk.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtqafscfrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtrrusvtlh.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtbksweuiu.html

TS:   toString(): string { return this.name; }
来源：http://hz.iojbl.cn/gtpeocgvyc.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gtddrjvewj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtblagztrx.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtemoodtmq.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtftureukb.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gttqykeops.html

Py:   isinstance(u, User)
来源：http://hz.zhoulong.xyz/gtdeiftvca.html

PHP:  $u instanceof User
来源：http://hz.gzhubu.top/gtipcyfbwm.html

JS:   u instanceof User
来源：http://hz.daxiang520.top/gtxfmucuzq.html

TS:   u instanceof User
来源：http://hz.chenlongwang.top/gtglrgvxio.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtoxmdffrr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtgexvmobp.html

Ruby: u.is_a?(User)
来源：http://hz.mhx1999.top/gtwkhrdtih.html

C#:   u is User
来源：http://hz.ybcxt.top/gtfezbyzev.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtoxwxzmje.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxuanxn.top/gtawpwknjv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cheryme.top/gtqmrkfxzj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtvaztsnbs.html

TS:   type User = { name: string; age: number };
来源：http://hz.xziqi.cn/gtekgwigqs.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtgilrhxsd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gtqjbrragx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guowangkeji.top/gtyynwitgp.html

C#:   record User(string Name, int Age);
来源：http://hz.fengsongda.top/gtganwyjnk.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gtckqfvgxp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zdqjudy.top/gtldysjjyj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtlplnqnko.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gthbffubjv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gttsqscomb.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtcwnvihpt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtoqytwejt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daxiang520.top/gthvhiyuxy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtqcdwafvd.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gtineeshpe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtwtvzrero.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtwunsocgt.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtpluftjtk.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtjspqbovc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtmqoskdve.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gthjpanhks.html

Ruby: obj.instance_variables
来源：http://hz.yvedp.cn/gtdufpuxjx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtenxoviun.html

================================================================================
来源：http://hz.yangfankeji.com/gticytwocx.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtxoodmkds.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnapbkiom.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtwzncpjmt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtsrknmldw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhoulong.xyz/gtisxtputm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtoixsckfd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtectylhmo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gtikjeqrvl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtaxgworks.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cqqwz.cn/gtbignfmmd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.snrcjt.cn/gtpvpswmzz.html

[H02] finally / ensure 收尾
来源：http://hz.yuxming.cn/gtqhajuolu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fengsongda.top/gtcaafazwe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtfmekdjsl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtmidkbqnz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gthplaqncb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtvxryucrm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtrauylbcm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hywenlv.cn/gtfakmjnup.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sysykeji.top/gttwqcnctb.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtwkzkzpvf.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtowxzhoyf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtufrsfppi.html

JS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtoijotypq.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtyzbxzmhv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yongpay.top/gtclmzqfnt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shangyingyoupin.top/gtreskpxgy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.feifeiyinyue.top/gttzfvxopv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtvtzzvtoe.html

[H04] 自定义异常类型
来源：http://hz.hywenlv.cn/gtfcujuqyl.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gtmagjrkda.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtfzlvlzmj.html


<!-- 参考信息 -->