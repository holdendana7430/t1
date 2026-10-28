代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gtcmsbayoo.html

================================================================================
来源：http://hz.hywenlv.cn/gtlvnzwzou.html

F. 文件与目录
来源：http://hz.fzhhl.top/gtysvfqdfa.html

================================================================================
来源：http://hz.yueranfly.top/gtypqrnevt.html

[F01] 读取整个文件
来源：http://hz.feifeiyinyue.top/gtcmczbxyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtqmyatyck.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xziqi.cn/gtifidfooq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guannengcc.top/gtvosbbmky.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yangfankeji.com/gtioxkgktx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtriywwgko.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtxskfbukb.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtuoxhrozm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtbmdyblek.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangkeji.top/gtjtqzpeox.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtwxgqurri.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.smart0.xyz/gthugisfje.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtshwrmaxh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtswgktsep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtixxnhlpm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtdiqlkggl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangtech.top/gtosrjlpgg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pycfn.com/gtvkksjegh.html

[F03] 写入文件（覆盖）
来源：http://hz.0kj1m.cn/gtwncebzrf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gtyepfgqpy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guannengcc.top/gtbjubexuc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtjhdrafri.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangkeji.top/gttixojuvy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtxcinsids.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.iojbl.cn/gtinbceuxk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yueranfly.top/gtbrzufmyx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guowangkeji.top/gttdeaoier.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gtxayvnwgq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuanzx.com/gtezrakuwz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtsdpktzlv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gticftclou.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtpfyzixcj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtbgyriryp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtliyfyuyy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtzrfgtnvp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.52xcode.cn/gtpypwywmf.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtpydnsvwb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.9152youxi.cn/gtemxfghhn.html

PHP:  file_exists("a.txt");
来源：http://hz.pengpengdd.cyou/gtkzuwrbba.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtjmalhzqe.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtdsrfzgwu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtswyddhvp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtmmjjarck.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gtxfwufkpg.html

C#:   File.Exists("a.txt")
来源：http://hz.chenjidiqi.icu/gtjqhjlmrw.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtvhwsudma.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtlhllhosa.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtzeacyrza.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtrpblwgdp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtrbjtcfzf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtvpotrzhy.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gttevhmldt.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gtmbuatuxf.html

C#:   File.Delete("a.txt");
来源：http://hz.zhongyouzk.top/gtvvjjfoho.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtzzmwhzke.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shzxlz.cn/gtvhfwjscy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.316326.xyz/gtcvmwdnaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtcotnvrei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtiaeybyyt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jyoumei.cn/gtclrqacfh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gogol.net.cn/gtqihzcavt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuanzhike.top/gtuhfekatp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cqqwz.cn/gtpsuwvznn.html

[F08] 遍历目录
来源：http://hz.52xcode.cn/gtmhbyhaor.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenlongwang.top/gtpjtkhmwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pycfn.com/gtjkujrmvb.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtfxtqkmfq.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtyxcojkfk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtmwwiankp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gttwqygvoa.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtfdjsuhpq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gtqhicnaxn.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtnevsixnr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtwewcpbpg.html

PHP:  filesize("a.txt");
来源：http://hz.ybcxt.top/gtfrtjtsgv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gteezqkujf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gthgdszmvk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtmxhrabfn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhengqikj.top/gthfnhcofk.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtlofdqnll.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jlsjyb.cn/gtupqoslnj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtkxjuzpmb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtiplhxxsu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtwtvxqnmj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtbwwyeezw.html

TS:   path.extname("a.txt")
来源：http://hz.gaohongyu789.top/gtzxjjpjtd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.havefunace.top/gtbrhqubdu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ppjwa.cn/gtfbcszguj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtsfbjihkk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gtwxspdycv.html

[F11] 复制与移动文件
来源：http://hz.fzhhl.top/gttptbfmgy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gthlyxkibo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gtyrpaevau.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtqcvomnzv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtlamisule.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtjfsyfwdw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenjidiqi.icu/gtxqqtcjwn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtbwbbriao.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sweek.top/gtsacwisao.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtzsbwuwcv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gaohongyu789.top/gtpsyuazou.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtlhgyjmzn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtcohrxlvr.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtuzsawyhz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtbptvdqos.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtgscnkfye.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sxryk.cn/gtedxybmjx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gthicevpfl.html

================================================================================
来源：http://hz.yuanzhike.top/gtgtxojund.html

G. 面向对象
来源：http://hz.jqgfzy.top/gtshiqaxio.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfvnnnpsr.html

[G01] 定义类
来源：http://hz.shuidangran.top/gtzqnufrqv.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtnohwnfet.html

PHP:  class User {}
来源：http://hz.ppjwa.cn/gtknsryfzr.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtspvnhuct.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtkcoglefk.html

Java: class User {}
来源：http://hz.jiagoushi.top/gtympbbiku.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtzjqxtogl.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtxxzzqywc.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtuwiwvqok.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtbhklsmqm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtrmbzdcpc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtklwznvjw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangdashe.top/gtanilrpfi.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtybkpzfdk.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtjlskmjhy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtwmfrfbpb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daria6918.cn/gtpbqpylkq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtugaemwos.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtabfqbzpk.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gthpkfgpmh.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gtqerzmyqt.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtfnyjczjd.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtzevumanm.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtyotvzqqi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtigcydvrd.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtrhfbzegx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtpsalocmu.html

[G04] 定义方法
来源：http://hz.nanxuanxn.top/gtfumkqvuv.html

Py:   def greet(self): return self.name
来源：http://hz.gogol.net.cn/gttzrobatv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtuizckagr.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gtjjfizrjb.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtcdpitvop.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtujiazuam.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gtdqoxakvg.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtforpxccc.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtcpvzzeqm.html

[G05] 继承
来源：http://hz.yj20258.top/gtomydkhoe.html

Py:   class Admin(User): pass
来源：http://hz.wangdashe.top/gtvgrvkwjd.html

PHP:  class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtqycwnldm.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtzngkktpx.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtuoupatni.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gtntcfmowe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gtsdmehvjz.html

Ruby: class Admin < User; end
来源：http://hz.yuxming.cn/gtnzkwxaxv.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtjkxpzquu.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtnauxjcqz.html

Py:   def greet(self): return "admin"
来源：http://hz.ydjk.org.cn/gtojmcknkx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtapuhtzhd.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtfcticfty.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtowukxepx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtrhagubru.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinyuanbaomall.cn/gtpagtytum.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtaouhhdmb.html

C#:   public override string Greet() => "admin";
来源：http://hz.haohaochexian.top/gtcyxcownb.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtckmdtsar.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtoeptzfcv.html

PHP:  parent::greet();
来源：http://hz.yuanzhike.top/gtjlidxrjp.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtyrowfymv.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtehleqpie.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtswiszlvk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtabwmlqxp.html

Ruby: super
来源：http://hz.jiagoushi.top/gtoqlffoxb.html

C#:   base.Greet();
来源：http://hz.shanyushiyangtech.top/gtcxekgcss.html

[G08] 静态方法与属性
来源：http://hz.wangshuangyany.cn/gtltiesgmm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtvjndgshd.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtshdujbpu.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtuxgldjys.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtlisyqqvf.html

Java: static void f() {}
来源：http://hz.gaohongyu789.top/gtuqvyxcxq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.havefunace.top/gtvhitmogg.html

Ruby: def self.f; end
来源：http://hz.nanxuanxn.top/gtacuitalz.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtarlxpqrf.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtgklcskqd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtnkycaoil.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yvedp.cn/gtjarhacua.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.redwolf501.top/gtstzaklkc.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gtzlnoxyvb.html

Java: interface Shape { double area(); }
来源：http://hz.cashguo.top/gtegndahgg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cheryme.top/gttkxkreva.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pycfn.com/gthzxwddug.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtcwcbzbfl.html

[G10] 访问控制
来源：http://hz.sweek.top/gtqsrnxkzs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gtnqcqaqjt.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtykvsydqc.html

JS:   #private 字段；其余公开
来源：http://hz.hongshengwenyu.top/gtqwxhyukg.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtdyiipozm.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtwldpzntt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtbvnwrsao.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtidjvcoaq.html

C#:   public / protected / private / internal
来源：http://hz.cucudq.cn/gtghqegumf.html

[G11] getter / setter
来源：http://hz.sweek.top/gtembnzcuw.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gttsonwshf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtydrchicz.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtstkllofw.html

TS:   get name(): string { return this._name; }
来源：http://hz.9152youxi.cn/gtoftpfsmf.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtlgqajeub.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ivvv.top/gtzgxkoduz.html

Ruby: attr_accessor :name
来源：http://hz.pycfn.com/gtuybyyxta.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtvfaocgfy.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gttkpkvhxb.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gtekejwzkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtbzqxsfja.html

JS:   toString() { return this.name; }
来源：http://hz.aibaodan.cn/gtzfsebeqs.html

TS:   toString(): string { return this.name; }
来源：http://hz.gzhubu.top/gtkwrzfciw.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gttusnetay.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtocxgievv.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gthafthpii.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtcfcyjnjh.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtwuqbhufz.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtoyittdxn.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtrxiisqdj.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtyzorqecl.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtncpywwcy.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtuikzazqx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtwmvxtoqx.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtxljqmyyj.html

C#:   u is User
来源：http://hz.haohaochexian.top/gthlrmweqk.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtefragjtx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhongyouzk.top/gtwykeojaw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtlfbbsfey.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gtitjhtnvx.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtqrwpslvo.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gtmlikumjb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.svipenyu.cn/gtuggjwokg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.52xcode.cn/gtddwpjuin.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtfhrwrhvu.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtkvtfdlwh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.9152youxi.cn/gtqozejfjn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtygrbignc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtedohtdiu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gthtkuskvn.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtgwfoohhw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.52xcode.cn/gtydponaor.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtuenqeupa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtjjtfkjfg.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gtraeknnvq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtetlfcore.html

PHP:  get_object_vars($obj);
来源：http://hz.shangyingyoupin.top/gtzzhsgund.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtydpukfyd.html

TS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtjotqftcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ivvv.top/gttgnqzbvn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtzpohlmov.html

Ruby: obj.instance_variables
来源：http://hz.dashuyun.cn/gtxpbmbpjx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtnijpkrad.html

================================================================================
来源：http://hz.aibaodan.cn/gtcncjtmvd.html

H. 异常与错误处理
来源：http://hz.yanxiufei.cn/gtleufbhvq.html

================================================================================
来源：http://hz.sufxvd.cn/gtohwmigft.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtvovfcahz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtkduyxvxa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtrobqkawh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtbhgkjhwn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gtojsuhmri.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtkrmlkmdv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtvxolpmvf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zycfv.cn/gtjjfvglhs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtobutmfct.html

[H02] finally / ensure 收尾
来源：http://hz.kuanghao11.cn/gttbqglfwi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtxjufyrvk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtwjwlakuu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtabvwdqfy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gticcubxos.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtgzrsbvwj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fengsongda.top/gtxlswkfnp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ivvv.top/gtmnjzdvkn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtqimsviay.html

[H03] 主动抛出异常
来源：http://hz.hfpthk.cn/gtfsnuehnx.html

Py:   raise ValueError("错误信息")
来源：http://hz.ppjwa.cn/gtkwgiggax.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtqtchdttm.html

JS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtypwhcrek.html

TS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtuodmrwck.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtgqcjaxyg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aizwys.cn/gtyxwozlul.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gtzbdwgwag.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtebukjupf.html

[H04] 自定义异常类型
来源：http://hz.chenzaomai.com/gtxztnkmyd.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtrzbzciuy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.c1oappe.top/gtpmxcsbrt.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtmqmqucmc.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtbzldvgej.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ybcxt.top/gtzqkzwriq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.9152youxi.cn/gtoadyscvg.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtqunxwpgs.html

C#:   class MyException : Exception {}
来源：http://hz.52xcode.cn/gtvanrecwf.html

[H05] 捕获特定类型
来源：http://hz.zhiwuduotai.top/gtxnvmhygi.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtelnulzgm.html


<!-- 参考信息 -->