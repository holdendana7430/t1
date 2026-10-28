代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gaohongyu789.top/gtfbrnhnzp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtgejcnxzi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtrcqllozo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtdjubkdbs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gthxssqshl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtdnfhgcfp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangtech.top/gtlvkocdyr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.9152youxi.cn/gtakcxmqij.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtlikiyxny.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtcctwsfro.html

PHP:  file_exists("a.txt");
来源：http://hz.yonumen.top/gtpajnekzp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtjfjryyce.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtbmyjjrzr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtlkaceqaf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtwnpgllwm.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtsqjtqlgx.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtuxopzrwz.html

[F06] 删除文件
来源：http://hz.yueranfly.top/gtthrxnosp.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtymuszlnt.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtforugytm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtdkslvmvg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtdhvusgwg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtyvghysbk.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtoerrwzzh.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gturvvslvv.html

C#:   File.Delete("a.txt");
来源：http://hz.gaohongyu789.top/gtkyhmwtbh.html

[F07] 创建目录（含多级）
来源：http://hz.ppjwa.cn/gtyoumljdu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtigjarqmy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dianchejie.cn/gtfpbwpekv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gthszhzizb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtniqrzmxh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gtpancmxox.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ywan-chungtsiang.top/gtrsluwoqt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtvfmhlspk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigfzy.top/gtkseutlli.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtxkqbchbe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.quarkkingdee.top/gtilbuzbyc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtsiyligxa.html

JS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtpvzynrjf.html

TS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtfffcysxc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtkmaziccg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtsrishedq.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtkrzkbley.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gogol.net.cn/gtjvlszecw.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtwowedeht.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnqzz.top/gtmfwqvflp.html

PHP:  filesize("a.txt");
来源：http://hz.jqgfzy.top/gtpiconfok.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtbijworxn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtfjzcionc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtvqljevli.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cucudq.cn/gtmwlzgwns.html

Ruby: File.size("a.txt")
来源：http://hz.meibo888.top/gtyorwasma.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.kuanghao11.cn/gtjkrxjcjy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtcoedlern.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gttzyffdln.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gtlenzeefp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtuegbpgki.html

TS:   path.extname("a.txt")
来源：http://hz.hnqzz.top/gtdrzdtpyh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangkeji.top/gtmhnyyysl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtpmaleknu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtrfbvuuhm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cheryme.top/gtaddntlhf.html

[F11] 复制与移动文件
来源：http://hz.gotoacloud.top/gtoalkzszj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtaihqmcan.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daxiang520.top/gtyjbafzxu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtnqmkejaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtvcnsyvux.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gthjjjoaqc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xylfe.cn/gtihargqpy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtghbntkjw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gthoohtstn.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtgnewoqbe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gttugswhpx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtbwoebgra.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtcdkuhbas.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtfkufngcv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gtkticnagt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ybcxt.top/gtmjdwugxs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtwfuqtyxd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.bjfxy.top/gthkecrqrc.html

================================================================================
来源：http://hz.yuanzhike.top/gtdfeagrfz.html

G. 面向对象
来源：http://hz.nanxinkj.top/gtcwblhkze.html

================================================================================
来源：http://hz.yj20258888.top/gtnwxbxehm.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtpyldfkvt.html

Py:   class User: pass
来源：http://hz.hywenlv.cn/gtggqykcbl.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtduwwgomy.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtogybwagg.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtplnvopwk.html

Java: class User {}
来源：http://hz.yuxming.cn/gtuddtfpei.html

Go:   type User struct { Name string }
来源：http://hz.tian-w.cn/gtxldyizgl.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtshxmhctf.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtmoqcfliu.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gtlxkapxgx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtsouotitg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtbdpfuvfk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtxjoqtkav.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtpcuucdgf.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtjcvhcjwe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gthckzjbst.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hywenlv.cn/gtnwysxoxr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aibaodan.cn/gtvvoizajm.html

[G03] 实例属性
来源：http://hz.kuanghao11.cn/gtolmbbuow.html

Py:   self.name = "x"
来源：http://hz.ivvv.top/gttykgnfup.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtzxiqkqdt.html

JS:   this.name = "x";
来源：http://hz.bjfxy.top/gtrsxxkgii.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtjvjcjqwn.html

Java: private String name;
来源：http://hz.chenlongwang.top/gteipstvfo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtlhimqbrw.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtbhiejhnk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtwfosddit.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtavtnylfb.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtolfcbvye.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtiqcaivyf.html

JS:   greet() { return this.name; }
来源：http://hz.hfpthk.cn/gtvyvnchqg.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtlwtdmchk.html

Java: String greet() { return name; }
来源：http://hz.zhengqikj.top/gtadlpzkuo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gthyvkberc.html

Ruby: def greet; @name; end
来源：http://hz.aizwys.cn/gtjzqunqcg.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gtiqrdqqtn.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtdbhopfgo.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtdjzyttxi.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtyvhpkdbv.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtfivgmsfa.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtwaiibjdz.html

Java: class Admin extends User {}
来源：http://hz.ppjwa.cn/gtrmjyzclx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gtvljxwnsa.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtymeqlrvw.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtlmvnylyz.html

[G06] 重写方法
来源：http://hz.yuanzhike.top/gthghrvkmz.html

Py:   def greet(self): return "admin"
来源：http://hz.quarkkingdee.top/gtmmjwysks.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtwzbaxexz.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtbyycfpsx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gthvaqqxyz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtdxpgxipn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtxntcpgsm.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtkblxeyuy.html

C#:   public override string Greet() => "admin";
来源：http://hz.52xcode.cn/gtxcxsqnyj.html

[G07] 调用父类方法
来源：http://hz.cheryme.top/gtglqcsmxq.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtvqhhsqhf.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtdonybpte.html

JS:   super.greet();
来源：http://hz.ppjwa.cn/gtjogqhoqu.html

TS:   super.greet();
来源：http://hz.ppjwa.cn/gtupddoprm.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtwobfhaig.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtomlyapbt.html

Ruby: super
来源：http://hz.aizwys.cn/gtstjmlusn.html

C#:   base.Greet();
来源：http://hz.yuanzhike.top/gteseijwas.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtpchtpocr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gaohongyu789.top/gtzfrnybii.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtluwynpdh.html

JS:   static f() {}
来源：http://hz.c1oappe.top/gtuidghqqy.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtizzhbinf.html

Java: static void f() {}
来源：http://hz.hammf.cn/gtqrombqvm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gtromxvfun.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gtyhkhhkxy.html

C#:   public static void F() {}
来源：http://hz.ydjk.org.cn/gtikhhkmqf.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gtkslqxcuz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jianghu66.top/gtpxeoesix.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenjidiqi.icu/gtcwgbbear.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gtecwazljv.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtpitzmbwo.html

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gtjngrpvut.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgufenzy.top/gtnfypkhab.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gtijamhmvn.html

C#:   interface IShape { double Area(); }
来源：http://hz.kuanghao11.cn/gtneibjkeo.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtkgbjbnzs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gtczyeigsq.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtdddwdjsd.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtedjrsnkj.html

TS:   public / protected / private
来源：http://hz.yuxming.cn/gtxhzwbswg.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgufenzy.top/gtnjzgfzxs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yongpay.top/gtdcvsbjfy.html

Ruby: public / protected / private
来源：http://hz.jiagoushi.top/gtrwvarvjd.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtyhwnrhjz.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtpvdhcgto.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtfvagzrwl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtnoajdhqh.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtfnktgzzf.html

TS:   get name(): string { return this._name; }
来源：http://hz.jyoumei.cn/gtzdzmygux.html

Java: public String getName() { return name; }
来源：http://hz.ydjk.org.cn/gtoylcjdxg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cheryme.top/gtqprxsbja.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtyqhsqaea.html

C#:   public string Name { get; set; }
来源：http://hz.zhaomingkeji.xyz/gtkkzzmvxg.html

[G12] 对象转字符串
来源：http://hz.fengsongda.top/gthgwpobej.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgufenzy.top/gtefpugsij.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtakunubpg.html

JS:   toString() { return this.name; }
来源：http://hz.havefunace.top/gtqwnjaqyj.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gttmzzmwlz.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtdivccqiw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtwxrsmyin.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtldgaseuq.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtgladpdiv.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtgvslzaqw.html

Py:   isinstance(u, User)
来源：http://hz.haohaochexian.top/gtozmmronp.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtdocgfuyf.html

JS:   u instanceof User
来源：http://hz.chenlongwang.top/gtwamgnspg.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtkxgmmyez.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtjqlbcpdn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.mhx1999.top/gtvvwkghdr.html

Ruby: u.is_a?(User)
来源：http://hz.zdqjudy.top/gtlpfaijka.html

C#:   u is User
来源：http://hz.jinqigufen.top/gtnxjiaaha.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtbbncmvpn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nwbrower.top/gtwksoxzsh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtmkwmrtti.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtqqncnqfz.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangtech.top/gtzizslbbz.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gthvykglwc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gtnmtvofck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtufiklafk.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtswtdcoaq.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtffsbfgyb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtyiyodtnd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtnfufaoia.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ivvv.top/gtwgdcuzix.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtpjwzqnim.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtneewqffx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cqqwz.cn/gtlhmqekhd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtwvfgpiws.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtptkyfqba.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtdhusojdd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guowangkeji.top/gtqjxxyaui.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gttefohzsp.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtigtaejam.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtphzaiibn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtiajywqmk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zdqjudy.top/gtumxxqxqk.html

Ruby: obj.instance_variables
来源：http://hz.zhiwuduotai.top/gtyedezfay.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtmczvwbpe.html

================================================================================
来源：http://hz.snrcjt.cn/gtcwloaxzl.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtloyqxrhd.html

================================================================================
来源：http://hz.xziqi.cn/gtmieeorxd.html

[H01] try / catch 基础
来源：http://hz.smart0.xyz/gtvrmswidj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtkpbtrisi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fengsongda.top/gtflaajjgt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtfjvlsthi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtnzbxihtf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gtmqltpjyo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtvvbxjcae.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtcvrfzzsm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gthbinmopb.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtjugfpwoa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtjvgbnbgq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtoxzpsyey.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtjcxmjckr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtrtxxjmxr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtobbguyuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtqaycpkka.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zdqjudy.top/gtshpbvudn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtbgvlbrzl.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtroqcxoyw.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtwzkwijua.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtkorshlhy.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtjljnkzkq.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtkhrisbmo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gtouxuqomu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtqwdbhria.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtwjvjsded.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtgvzbgyyb.html

[H04] 自定义异常类型
来源：http://hz.yangfankeji.com/gtptugfqyp.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtqzxtiguc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtpaodhuyt.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtnybncryr.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtdhbodygi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtlcbvlfoh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gthlchjskv.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gthrojwsjj.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtacsmvatz.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtsuojrooa.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtoipyqwqq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenlongwang.top/gturrhxcsm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtgqiavmjr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtmseaytqn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.iojbl.cn/gtglmabnxc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yonumen.top/gtoaedachq.html

Ruby: rescue ArgumentError => e
来源：http://hz.ppjwa.cn/gtdyegtuvj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yueranfly.top/gtgzugohee.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtprfbnozh.html

Py:   value = d.get("k") or default
来源：http://hz.ybcxt.top/gtajjwkwlr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtibqwgvqn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtwrpamwdm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtyyucmhpk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydjk.org.cn/gtnmsiqnyd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zycfv.cn/gtdalwysqx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtmdxhnnsi.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtffnsvqap.html

[H07] 断言
来源：http://hz.birdmap.top/gtbvbdmxat.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtkjvwrjoi.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtpptbgkbi.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtecwyszkj.html

TS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtbeiferji.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtoviabmcr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuxming.cn/gtqayyqboe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gttpnvkjwt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gttnlwfyvi.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtxsjwdszc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhixingplan.top/gtwtgiijyu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtuxrpbjww.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gtxjwxfdbp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhixingplan.top/gtvpdrhlzp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtvijvhhvv.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtxxukbpml.html


<!-- 参考信息 -->