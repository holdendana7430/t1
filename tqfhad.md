代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gttysylzrl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhaomingkeji.xyz/gtuicudqqh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtnytaeuhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtmssdcsgr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gttlyyjhgb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.c1oappe.top/gtokdhhrtw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtrtjqdspa.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxinkj.top/gtfyfuvzje.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hongshengwenyu.top/gteumitkjo.html

================================================================================
来源：http://hz.zdqjudy.top/gthstelxdr.html

F. 文件与目录
来源：http://hz.tian-w.cn/gtpvowzjeb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzexkqsdv.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtqmkbivuo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gttvjvhhce.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenlongwang.top/gtpgygocpt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hammf.cn/gtdvkogsfs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yueranfly.top/gtvglohxyu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtlxkjugmu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtwuuoyxmt.html

Ruby: File.read("a.txt")
来源：http://hz.chenjidiqi.icu/gtigspgtal.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xylfe.cn/gtipmdipmu.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtolamsvoe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hfpthk.cn/gtcmyzexup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gtngbhkymo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtdnqvosyu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gttdnbifdc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shuidangran.top/gtebvhizzm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenjidiqi.icu/gtadztgfpx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtigmncfec.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtoiebyddn.html

[F03] 写入文件（覆盖）
来源：http://hz.ybcxt.top/gthwadllvp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtgenhkezp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtnxvhocqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtexuydpso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtqpeulhgn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gtcbvydoml.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sweek.top/gtbhrbqucl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtczgndpji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jiagoushi.top/gtljwwlugy.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtibkqrysj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nanxuanxn.top/gtexpixtkd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtdovyylvh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtdzgsiztp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gthievbbrz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gthfijtqia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenzaomai.com/gtfreduljr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigfzy.top/gtpxmprkbf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.haohaochexian.top/gtcwyffqyu.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtljbtojfl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtkiejdfpd.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtappnaeec.html

JS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtutlrifix.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gteyktjnym.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtksxcocli.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shangyingyoupin.top/gterayyxdj.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtiatuvwnl.html

C#:   File.Exists("a.txt")
来源：http://hz.yanxiufei.cn/gtandydfps.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtaemkmnxd.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtsicoqctx.html

PHP:  unlink("a.txt");
来源：http://hz.zdqjudy.top/gtfihwcpgr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtrrcahaex.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtamjbniho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtwuwgclkt.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtcsiwpzyz.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtpapeeevl.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangtech.top/gtmptwbulp.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gttctwckbo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtybgtrqvq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hammf.cn/gtcupzdtrv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtlnfbudns.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtsapocuhj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cqqwz.cn/gthtptluxr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj202588.top/gttgrwhbyp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gtzcvzicon.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zdqjudy.top/gtcgznrhzc.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gteveomath.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxinkj.top/gtxzbuxlji.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtrzoqairo.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtkwuwhhzw.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtcoododbn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtfapxjejm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtekwiucgq.html

Ruby: Dir.children("dir")
来源：http://hz.jinyuanbaomall.cn/gtlxfkpebt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhixingplan.top/gtgmarqmni.html

[F09] 获取文件大小
来源：http://hz.fzhhl.top/gtekmydurm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtcjmamult.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtywjfhhwf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtzokwypyb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtltluoefw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtzszdzoae.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtnchaqsff.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtwyjrtsyk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhixingplan.top/gtlwnytttj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtekcwborc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtkxhdqazs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtdxrvcmdx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtwacymgux.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gttgodpmxl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cucudq.cn/gtwwspuavi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtzdzzdufk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtzspadzkj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtnmeroenl.html

[F11] 复制与移动文件
来源：http://hz.nanxuanxn.top/gtyodrpipx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtmsmmcqna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.havefunace.top/gtddiyvvtp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtsqsispaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtcwrclqds.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtlgmfnwao.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtpdnhgwda.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtxzbuztjt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtgeetgoax.html

[F12] CSV 读写
来源：http://hz.yueranfly.top/gtjcynjkar.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhengqikj.top/gtahxasnpj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gthwctfuml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtyitwepwd.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtnvpqyild.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.0kj1m.cn/gtbpzjykyo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtdbbupxtm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhoulong.xyz/gtfassyffu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shangyingyoupin.top/gtmapwkrqc.html

================================================================================
来源：http://hz.hnqzz.top/gtigywfjqh.html

G. 面向对象
来源：http://hz.meibo888.top/gtobszkhpw.html

================================================================================
来源：http://hz.yj20258.top/gtoyedkwcg.html

[G01] 定义类
来源：http://hz.xylfe.cn/gteenszfaj.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtfhjigamw.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtjxoeifef.html

JS:   class User {}
来源：http://hz.hongshengwenyu.top/gtzstyeiyg.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtpzhjokcw.html

Java: class User {}
来源：http://hz.xuanzx.com/gtwmtftlih.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtpcfjeahs.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtnmqlsiyo.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gtfzkihabh.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gtauqmjded.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gzhubu.top/gtykzpfomy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtodwdndte.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtwvafdrru.html

TS:   constructor(public name: string) {}
来源：http://hz.hongshengwenyu.top/gtrfktwgoa.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtboyyenst.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtyohhbodp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.smart0.xyz/gtwrtmsaua.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gthhshjtgf.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gttiyzolaf.html

Py:   self.name = "x"
来源：http://hz.pengpengdd.cyou/gtfhesltvk.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtzfjxeifx.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtppqzyylz.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtfjnwfnny.html

Java: private String name;
来源：http://hz.daxiang520.top/gthqngocbc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtbfnfdyng.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gteqhlvyou.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtgsacnqnz.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtiangzmci.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtfvqxhfws.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtvrkfytrb.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtyuevajjc.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtksdclbrb.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtkpxjtuzi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtoiuprkos.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtjkwmtkst.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtgvtojvqq.html

[G05] 继承
来源：http://hz.xziqi.cn/gtpczqpara.html

Py:   class Admin(User): pass
来源：http://hz.dianchejie.cn/gtiyacppgv.html

PHP:  class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtfcyoczht.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gttionqvxm.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtttzgfjud.html

Java: class Admin extends User {}
来源：http://hz.yongpay.top/gtyhxhjeed.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtmpdwykxd.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtchlvlhlw.html

C#:   class Admin : User {}
来源：http://hz.jinyuanbaomall.cn/gtefumtzik.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtwpavfmmv.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258.top/gtjkllnecp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtwzgikiuc.html

JS:   greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtrjiynceo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtexbqilub.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.havefunace.top/gtniavdomb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ppjwa.cn/gtdvfocjgq.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtkqxfhzlp.html

C#:   public override string Greet() => "admin";
来源：http://hz.xziqi.cn/gtalfzzxot.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtewfitluj.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gturyqhwwf.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtdfttmvyk.html

JS:   super.greet();
来源：http://hz.daxiang520.top/gtdtwxiehb.html

TS:   super.greet();
来源：http://hz.aizwys.cn/gtzcxgygrz.html

Java: super.greet();
来源：http://hz.svipenyu.cn/gtcdhziuyn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtcpmzpgad.html

Ruby: super
来源：http://hz.daxiang520.top/gtaqzvzdss.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtkuoocjyg.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtogmsyhpe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.kuanghao11.cn/gttlbrzpjk.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gthuvxrlsa.html

JS:   static f() {}
来源：http://hz.gotoacloud.top/gtsyshvfyk.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtmapwepvi.html

Java: static void f() {}
来源：http://hz.316326.xyz/gtqemiiggf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ivvv.top/gtsmktksqi.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gthpmrtqcf.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gtlyibuykm.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtpufffjqk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gthmffxgab.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtwquzsiyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigfzy.top/gtedeohxim.html

TS:   interface Shape { area(): number; }
来源：http://hz.cashguo.top/gtbonhvyhr.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gteejqcziy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtwkxbbxao.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtamvvlagb.html

C#:   interface IShape { double Area(); }
来源：http://hz.ybcxt.top/gtmnmdepgx.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtaiyrztyc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtcsvbmsqj.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gtnqefgyec.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtclzxqbno.html

TS:   public / protected / private
来源：http://hz.hywenlv.cn/gtvdlydsql.html

Java: public / protected / private / 默认包级
来源：http://hz.ydjk.org.cn/gtpkbublwg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtnjemshos.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtgpoahyyp.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtziprnhrb.html

[G11] getter / setter
来源：http://hz.cucudq.cn/gtunswgvsl.html

Py:   @property 与 @x.setter
来源：http://hz.zhijiandao.cn/gtwsdtaokz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtgrnmctnh.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtmwdtiydp.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtqkkmmiww.html

Java: public String getName() { return name; }
来源：http://hz.aizwys.cn/gtyqqqrpyw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gtcauvshzg.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtvyskpxzn.html

C#:   public string Name { get; set; }
来源：http://hz.yvedp.cn/gtganugvzj.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gtjfxkqsun.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtlsiriswi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtzccfpwgm.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtcsfwuhnj.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gtbtyzaawn.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtvprcsdmu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cdnleiting.top/gthobakvab.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gttpunsvmm.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gtvyoyzadt.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gttguujmwr.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtnfeoobbx.html

PHP:  $u instanceof User
来源：http://hz.aizwys.cn/gtnbdpjvgj.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gtpracisna.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtsppyxktq.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtysbucaow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xingfuxueyuan.xyz/gtnzsgdamk.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gttpotkmdm.html

C#:   u is User
来源：http://hz.cucudq.cn/gtosazgcmj.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtkjeletdd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtuykgbmsb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.havefunace.top/gtydezrtxg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtgzlomkpi.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtewvodyin.html

Java: record User(String name, int age) {}
来源：http://hz.yueranfly.top/gtwstuncbo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gtoateliwl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtvnbsqkfx.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtzikccwwk.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtqtivfvei.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtbzzqlatk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gtyyqhcwzq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtopfpeojm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtnurrlbco.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtszthbtds.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtejysjqpg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangtech.top/gtqcjupzeq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtjezploay.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigufen.top/gtvjibtbil.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtxxfhywxq.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtrpcgldcv.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtilvcfwil.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtrrdwpnnr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gticracnrb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jlsjyb.cn/gtmojcnwlr.html

Ruby: obj.instance_variables
来源：http://hz.yuxming.cn/gtlvaljwtr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtfakxsmby.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvzgjinmh.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtdnkkzexo.html

================================================================================
来源：http://hz.jiagoushi.top/gtyjdoypgd.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtqgbnacdt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtzxyfsbhz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtuzhpmszb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtutfxjkoj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtipfrvtnm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtptxlxube.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtmmxftphb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtmewsbpfn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tanke756.top/gtgvmtkdiv.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtgdwuvmha.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgfzy.top/gtgvasdslo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtspgcuvff.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtcbumunmt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtekzzylux.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtnwctiybi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gttjzedlpq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtxcexbrfg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.quarkkingdee.top/gtyrotysuv.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtqmzfohkx.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtubavzpnv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.birdmap.top/gtfybfocke.html

JS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtdmsmyjqu.html

TS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtxzrnguvq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtquownnrx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xingfuxueyuan.xyz/gtqpzarjjj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gtxdwxusnl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtkziaigqm.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtzhfqkarj.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtqrgzadoa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtmnppdoan.html


<!-- 参考信息 -->