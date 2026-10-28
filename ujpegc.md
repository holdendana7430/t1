代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yueranfly.top/gttcjodizr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrxoqswul.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtyntseyhk.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtoyuiwszc.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtxblchsby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtexdcbuol.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtjvemffuk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtzviiavxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigufen.top/gtajnudppz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtmoklgzcl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtqnenmhml.html

Ruby: File.read("a.txt")
来源：http://hz.ppjwa.cn/gtbyppsumf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hywenlv.cn/gttnvuadyr.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtblrozeng.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.svipenyu.cn/gtwgtencbb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cdnleiting.top/gtqxbgemxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtteggjpwy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtmbblrtrz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtcceloxpv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xziqi.cn/gtnqzfephl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtawbkfehr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.daxiang520.top/gtqazcfrcp.html

[F03] 写入文件（覆盖）
来源：http://hz.bjfxy.top/gtsoantitj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.snrcjt.cn/gtqvxyneat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtmkmmaxpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtwhljfeia.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtjjptsbkl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guowangkeji.top/gtlriyrfzv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtariuuqyd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gtobkvziab.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gttdxlqjoe.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangkeji.top/gtvtioxfed.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shangyingyoupin.top/gtjifdtkpj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtelmidnhr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtqadnryqt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtweoosnbu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gttpdyrbal.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258.top/gtzgrctwzv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cucudq.cn/gtkchyejbv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtsvzfnogg.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigufen.top/gtiejuibhn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yangfankeji.com/gtznbfelhz.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtgfnbzhvd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtuqzpxtks.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtlyoxubkg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtlgphnivx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gzhubu.top/gtusksptzv.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenjidiqi.icu/gtxworlsrs.html

C#:   File.Exists("a.txt")
来源：http://hz.cucudq.cn/gtgjfnjlvr.html

[F06] 删除文件
来源：http://hz.jlsjyb.cn/gtgwdhzdzw.html

Py:   os.remove("a.txt")
来源：http://hz.aibaodan.cn/gtclvaghnq.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtzwnloffv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtldksauwg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtsnsgvqve.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtrasxxxsz.html

Go:   os.Remove("a.txt")
来源：http://hz.sweek.top/gtnqvzmmtp.html

Ruby: File.delete("a.txt")
来源：http://hz.ivvv.top/gthjnfmwfk.html

C#:   File.Delete("a.txt");
来源：http://hz.aibaodan.cn/gtpcfovymd.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtdcsqlovl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guowangkeji.top/gtbywavugd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.0kj1m.cn/gtdcbljilq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtelymwrrn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtykytzdxi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.quarkkingdee.top/gtnoijsdpt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cashguo.top/gthvuyfyei.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gthldyarnk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtdxgpgcku.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtmcvcvllv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtosasgsap.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtcwijoyzq.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtighublzy.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtuhytihti.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gthgroinzf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtfdzrrsyi.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtwodavbcz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtrluuyyaa.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtmvqoqjvq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhengqikj.top/gtdwerqfoq.html

PHP:  filesize("a.txt");
来源：http://hz.yuanzhike.top/gtkdylhghj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtalutence.html

TS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtlmmbojkc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sweek.top/gtpfbbzvti.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gaohongyu789.top/gtqcvidvsj.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gtlngkhsac.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtaoyaxmoc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gtvmlwxjqq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtvbxepoag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnqzz.top/gtqkbuxjuv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtlfvjjkhd.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtswmftpoq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gteachioxa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtxqqmtpsc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtysatotvc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtsnfuhmzc.html

[F11] 复制与移动文件
来源：http://hz.ivvv.top/gtdhiwevry.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtejcsiqhv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtiezwxyjh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtdomuosio.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtyzxwwmla.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxuanxn.top/gtihoxqupz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gtxvcamubw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtslhrlsje.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtcxqwvqqx.html

[F12] CSV 读写
来源：http://hz.jlsjyb.cn/gtxwchlfdm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shangyingyoupin.top/gtgswrcsua.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtzttxfkru.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtbzyvxtll.html

TS:   // 同上
来源：http://hz.hongshengwenyu.top/gtgyzxliha.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gtzrqpkypf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.52xcode.cn/gthszfjdlm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtedwvuday.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtnxyawfca.html

================================================================================
来源：http://hz.jinqigufen.top/gtwrtvqirs.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtyawvvjgn.html

================================================================================
来源：http://hz.zhengqikj.top/gtaouwwmcj.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtedftmzag.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtsiiwvcbh.html

PHP:  class User {}
来源：http://hz.yueranfly.top/gtxwddstzl.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gtxmihffse.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtbfawuuaa.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtalthjuww.html

Go:   type User struct { Name string }
来源：http://hz.zdqjudy.top/gtfivhlqlg.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtmpcycagm.html

C#:   class User {}
来源：http://hz.jqgufenzy.top/gtooakmmte.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtfarptxxu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gtyolzcblb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gtrgazkepd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtzahqroak.html

TS:   constructor(public name: string) {}
来源：http://hz.gogol.net.cn/gtsfdtxjux.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtlvgmgppo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258.top/gtthzdmkqd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtldigzwyy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtlwmgzesu.html

[G03] 实例属性
来源：http://hz.ehwqpu.com/gttrtudgey.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gtikjcglza.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtqurwiqac.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtmahfyldc.html

TS:   name: string = "x";
来源：http://hz.xylfe.cn/gtqubrldly.html

Java: private String name;
来源：http://hz.sysykeji.top/gtkztqpvnz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtcloirqfi.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtteqjvsdu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtmujjoyqb.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gthaecuibw.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gtkhklbrjk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtmjwrgxrh.html

JS:   greet() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtqpvyejgy.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtguwtwflz.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtatanaqhk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gthdwkudnz.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gtbpbdqtqc.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtwlsbspsv.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtvogpxeiz.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gtrizzlbiu.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtgmubyalj.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtfzdaccsw.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtgwvyyeid.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtwmrnxhqr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zycfv.cn/gtocobndkf.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtpifonzjn.html

C#:   class Admin : User {}
来源：http://hz.hammf.cn/gtowbcktxv.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtsfoojliw.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtpckcwfps.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtkhrrogxc.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtccjzyulb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtggywtejf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtvflfoerr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.meibo888.top/gtoxqgszqx.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxinkj.top/gtdrfevbwd.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtqmhlmpbr.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gthqijhaoc.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtmazbkrcj.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gtxblvpfsr.html

JS:   super.greet();
来源：http://hz.yj20258888.top/gtejwqzefa.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtvqlzkgpm.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtwinclusn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtlldkykwi.html

Ruby: super
来源：http://hz.jinqigufen.top/gtgjnvdrmr.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gtxbsbjdkq.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtjiutcqjo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtskszpadg.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtlzjoxadx.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtrbfqbpxz.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtxdregsak.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtwfsqmvur.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtbaduuhxp.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gtuwuqncfe.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gtixeruhsc.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtbebedrts.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.quarkkingdee.top/gtoiomzuls.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj202588.top/gtltmbuyce.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtuswuuvsq.html

TS:   interface Shape { area(): number; }
来源：http://hz.0kj1m.cn/gtrulspjha.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtxxfpgfbm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtfmzbjjcc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtxvwlgohc.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtjxsakljf.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtzxrifdkx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtbbmzviok.html

PHP:  public / protected / private
来源：http://hz.zdqjudy.top/gtpbyeoolp.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtgubinpnm.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtvpvvgynw.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtuvylhvfc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtnnjllaxk.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtdzyneyxw.html

C#:   public / protected / private / internal
来源：http://hz.wangdashe.top/gtwwlxsbpy.html

[G11] getter / setter
来源：http://hz.yangfankeji.com/gtyxvafxqg.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtnaydufdc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtoxmxpggn.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtvncycxog.html

TS:   get name(): string { return this._name; }
来源：http://hz.vqdsnc.cn/gteyumorcc.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtjwkxylkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtawcypbff.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtenodrzra.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gtpmmzopok.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtjrkzuslg.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtmlnbmxdi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtxbxzmori.html

JS:   toString() { return this.name; }
来源：http://hz.redwolf501.top/gtsngktnah.html

TS:   toString(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtmxulinjt.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gteumztzlf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtbllvpsfe.html

Ruby: def to_s; @name; end
来源：http://hz.fengsongda.top/gtusybzdqk.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtxhjkessv.html

[G13] 判断对象类型
来源：http://hz.shuidangran.top/gtyxrkssqi.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtysolkkyn.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtwshgumtv.html

JS:   u instanceof User
来源：http://hz.hammf.cn/gtbckyxhsa.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtxebtpfhq.html

Java: u instanceof User
来源：http://hz.jianghu66.top/gtazcpphol.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtvqccnzka.html

Ruby: u.is_a?(User)
来源：http://hz.zhongyouzk.top/gtqnqyjxmg.html

C#:   u is User
来源：http://hz.cashguo.top/gtdbykluuc.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gttyxyepcb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtexeupejv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtqeggyfpk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gtpwtqvlwy.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtwjikntuw.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtstzsqyem.html

Go:   type User struct { Name string; Age int }
来源：http://hz.quarkkingdee.top/gtatjastoe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtziipzwhq.html

C#:   record User(string Name, int Age);
来源：http://hz.ybcxt.top/gtnlquevae.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtjdvldaew.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xingfuxueyuan.xyz/gttqnqkiuk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hysaishi.cn/gtacecmwta.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtbljwzieo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtbhzgiqpy.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gtpjoxhvpw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtvnxpelzu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtwgviwkij.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtmgvemyqo.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtuchghuyn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtswdgiofl.html

PHP:  get_object_vars($obj);
来源：http://hz.xziqi.cn/gtbbexjdic.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gterpdqvnk.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtfiblqhce.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yvedp.cn/gtfoqnelct.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtveaasbyk.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gtawixqdxv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gthbwndzsh.html

================================================================================
来源：http://hz.xinyue.icu/gtsrfvkaqc.html

H. 异常与错误处理
来源：http://hz.yanxiufei.cn/gtgmgdiemm.html

================================================================================
来源：http://hz.jqgfzy.top/gtgpudcmft.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gtnuulndvz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnxiangtu.top/gttgydrbzs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtzxwhbdnu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtyuylsfhr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtmuomrocv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.0kj1m.cn/gthrghhgtb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guowangkeji.top/gtamzsuymv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtlhbuousg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtblrjnqhk.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gteawjtqwb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtecraleoj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtedcxackm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtnyxxhrqy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtrasazzub.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtijkojyln.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtifnprqoo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtlcpqydal.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gtbpuuiyiy.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtrnyjquds.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtqbchyemu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtbcenkrpi.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtlcfbfuqh.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtpxzvjufu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtzlcalarj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shangyingyoupin.top/gtuakogkdm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gtzhvpyfpx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtaivsuktw.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtnizllueh.html

Py:   class MyError(Exception): pass
来源：http://hz.hywenlv.cn/gtkxbjzwpz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nwbrower.top/gtgxwhwapz.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtelgkcuuc.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtjlqwmlwo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtdgtkbjmd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnqzz.top/gtjtiiacct.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtnzgiohzp.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtdpeyccej.html

[H05] 捕获特定类型
来源：http://hz.cdnleiting.top/gtwdutrvzt.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gtfidailpw.html


<!-- 参考信息 -->