代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gtauiayjhj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtyhoibyel.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtdnyhwcvl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtmpcpmihl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtwrqrbpem.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tian-w.cn/gtkzyrqefa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtziqbgzil.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtlxbybvad.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtnxitgbmc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtcxwlwrqn.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtuuvapizs.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtfhgbcwkc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtujdaftzx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtqskvcrzw.html

Ruby: Dir.children("dir")
来源：http://hz.svipenyu.cn/gtohtkqtqk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtbhliasyd.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtbfswwlxr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtfzibhzev.html

PHP:  filesize("a.txt");
来源：http://hz.52xcode.cn/gtpbuuuxxm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtblderpeg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtdbkojwhu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtjsfjiict.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gaohongyu789.top/gtfqoenoll.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gthtoebsxb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtkgmditqs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gtgspvlkfc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtsdfirutw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangdashe.top/gtgsrhswgm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtaefoonai.html

TS:   path.extname("a.txt")
来源：http://hz.jqgfzy.top/gtutovnydd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nwbrower.top/gtzvzvysbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.c1oappe.top/gtvcwhxtvj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gttnzznrrp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtudyzfjyh.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtvpwqhytm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtqgtyqczz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daxiang520.top/gtqxueregl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtrdodszlh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtzbhncvdo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhijiandao.cn/gtyqsenina.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtvsancgqj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtbppmusfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtmxaiejoe.html

[F12] CSV 读写
来源：http://hz.svipenyu.cn/gtuxqwoopo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtjloqgztw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gthumfbyse.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtiaakurty.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gtqtuanrro.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xylfe.cn/gthznsyoxq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtwgpzpfrr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtwimoxnhm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtehkbkawu.html

================================================================================
来源：http://hz.yj202588.top/gthxymhvuq.html

G. 面向对象
来源：http://hz.gogol.net.cn/gtugntnqxf.html

================================================================================
来源：http://hz.iojbl.cn/gtjpnrxkrt.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtqsmpzpgp.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gtxvbudqse.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtaegxenfj.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtuknmognr.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gthvjlofqb.html

Java: class User {}
来源：http://hz.haohaochexian.top/gtccpgrynu.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtxmnyysqf.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtwklcyqqo.html

C#:   class User {}
来源：http://hz.chenjidiqi.icu/gtdctdnsjx.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtoqzffqfj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtnrcuxbza.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgfzy.top/gttyxoxeqr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gtdsscynjl.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gtlevcuqyk.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtllsnpowx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhongyouzk.top/gtcvgwmubd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtwfrjygsq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dianchejie.cn/gtzvmglzce.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtblzkfhvy.html

Py:   self.name = "x"
来源：http://hz.sxryk.cn/gtnletfpya.html

PHP:  public string $name = "x";
来源：http://hz.jqgufenzy.top/gtsvpqjhmh.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtdzpnrrhj.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtlqoccxxu.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gthgeszkwn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pycfn.com/gttjuljmhc.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gtfnbijrcc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtbraalxjj.html

[G04] 定义方法
来源：http://hz.cheryme.top/gteprlalmm.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtmgjwsqaw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtiiurxpth.html

JS:   greet() { return this.name; }
来源：http://hz.aibaodan.cn/gtknjggodj.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtrhzqqbbo.html

Java: String greet() { return name; }
来源：http://hz.svipenyu.cn/gtqyvoswwl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtwzhnqnmp.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtnidfcxdq.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtvycnuhtu.html

[G05] 继承
来源：http://hz.cheryme.top/gtwumiejpm.html

Py:   class Admin(User): pass
来源：http://hz.yonumen.top/gtjrpfbjpm.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtxckymyih.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtqlifgvnr.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtkypyjneb.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtzxughaxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtphhcrerk.html

Ruby: class Admin < User; end
来源：http://hz.tanke756.top/gteoxkpdqo.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtmgntkjef.html

[G06] 重写方法
来源：http://hz.birdmap.top/gtfrbzxmum.html

Py:   def greet(self): return "admin"
来源：http://hz.tanke756.top/gtgnsmsenh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtezsrrtqk.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gttwdlerjs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtwsquddkm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258.top/gtokiclyej.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuetiantiany.cn/gtdutchyjq.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtrkjwvxfy.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gttydebkzv.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtrykkrain.html

Py:   super().greet()
来源：http://hz.chenjidiqi.icu/gtyvcenjml.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtlmagntwt.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtsiqrvcub.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtdafstcmp.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtpysomsac.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xylfe.cn/gtdkjerfxe.html

Ruby: super
来源：http://hz.ppjwa.cn/gtsembqwed.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gteldueahu.html

[G08] 静态方法与属性
来源：http://hz.xuanzx.com/gtjyxpufxa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtwxxqujog.html

PHP:  public static function f() {}
来源：http://hz.c1oappe.top/gtargazaec.html

JS:   static f() {}
来源：http://hz.shzxlz.cn/gtkhndrrrx.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtmfwnsjab.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gthfkmyfpo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtjzcmirqg.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtzufvogeg.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtbbfwobic.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtznalkynj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtndhjplyu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtgqyhdycd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gttssoouqq.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtfoxflybc.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gtbzvwzxoh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cqqwz.cn/gteaaahkry.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtbhjjfbde.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtzckwudwn.html

[G10] 访问控制
来源：http://hz.sufxvd.cn/gteybfmtwm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jyoumei.cn/gtqkqmacqr.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtbihczjvi.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtciqwkakx.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtmqrhioez.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtqogjjhsd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtxyxidnpq.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gttkhofkym.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtkqsgycmm.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtywejvreg.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtiaoyzmew.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gthnvdorkz.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtfchzgwgu.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtvqjsvmhh.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtgribktoi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtczbmqdkd.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtugmdvpro.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtnbnklbax.html

[G12] 对象转字符串
来源：http://hz.ybcxt.top/gtmlvzbybw.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtzxrixvjn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtizsaqaiy.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtkjrjacac.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtnradbrhn.html

Java: @Override public String toString() { return name; }
来源：http://hz.hammf.cn/gtbsfgeicm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtwgcqmzjl.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtsbnoipck.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtnyolmtst.html

[G13] 判断对象类型
来源：http://hz.hnqzz.top/gtxvbacmfb.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtjavkqmay.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtxjfrhooe.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtpwcwtjct.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gttojbxwey.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtekwbcbor.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinyuanbaomall.cn/gtffpggeht.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtcvyvdqie.html

C#:   u is User
来源：http://hz.sysykeji.top/gtaltrbmfm.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtlqxclxng.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtryrbazzg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtwuagprpr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtdylnwqap.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtjkzzpohg.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtuixmtdpw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtrhfkfycx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xylfe.cn/gtkjkqshur.html

C#:   record User(string Name, int Age);
来源：http://hz.0kj1m.cn/gtlirgwofn.html

[G15] 枚举
来源：http://hz.yj20258.top/gtyoauocyd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gtolsemkbd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtpjzipixx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.quarkkingdee.top/gtyfoojqlk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtfpvfpirq.html

Java: enum Color { RED, GREEN }
来源：http://hz.ybcxt.top/gtintsgwmf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtrirabrno.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hfpthk.cn/gtgkvpxwgu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtkgduexko.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtarkmqwtb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj202588.top/gtiuujpfiz.html

PHP:  get_object_vars($obj);
来源：http://hz.pycfn.com/gtbqwmafvm.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtysnwfjwi.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtvdxgcbmj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.quarkkingdee.top/gtxifkxivn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtltrscknw.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtrhmqfzra.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxuanxn.top/gtddfigclh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtogbufnpk.html

H. 异常与错误处理
来源：http://hz.shzxlz.cn/gtbneuzvcj.html

================================================================================
来源：http://hz.aibaodan.cn/gtdaqdshtb.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtctdxumat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtixdxmykk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtveecexcz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtivpsgeme.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xziqi.cn/gtthasmupn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gtbkeddkxr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.havefunace.top/gtitmyibjs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gttnxqqicn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtabrrrejf.html

[H02] finally / ensure 收尾
来源：http://hz.yj202588.top/gtzipnrtgp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenlongwang.top/gtxxvnbtmx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtlsdzjicc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtqwaxpoxk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtnhbguxaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtsnrtvpoz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gtwgqtgdok.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gtwkhbswlf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtaymbsxpe.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtsgveqiyq.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenzaomai.com/gtybzfozfa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtembntfsn.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtmqfebxbe.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtpxtvwjis.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gteingfhym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ybcxt.top/gtjwfrqgpv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtlvnwmxtv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gttpsltrbh.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gtdhvuiqnt.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtznupyyff.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtbtrwpbsk.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtsewekhle.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtqckivlhh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtyascpgsg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenlongwang.top/gtqtnmmkyv.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtuwelbfwc.html

C#:   class MyException : Exception {}
来源：http://hz.yongpay.top/gtejdrvmzx.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtuwjmaalu.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtsiiutakx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtbnxktpus.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtyqzckfoh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtdiashdpw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtkduepjvv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gtzmqmtcej.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangtech.top/gtyazfvehu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nanxuanxn.top/gtsdxxbcxj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cheryme.top/gtbrmylqwq.html

Py:   value = d.get("k") or default
来源：http://hz.zhaomingkeji.xyz/gtsrjahnak.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtlpcpdryc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtlgrtftoi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtygejbjbn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtflbqxkoy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aizwys.cn/gtymthwvij.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtubednyuz.html

C#:   obj?.A?.B ?? default
来源：http://hz.sufxvd.cn/gtzikbdtsh.html

[H07] 断言
来源：http://hz.chenlongwang.top/gtbdexokvh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtiokuilxt.html

PHP:  assert($x > 0);
来源：http://hz.jinyuanbaomall.cn/gtzqlophjv.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtzmzdthcb.html

TS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtuspfqmpf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.9152youxi.cn/gtgzujdphg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtskcofkch.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.52xcode.cn/gthfdemjak.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtckcqgbbs.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtlvszrgur.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shzxlz.cn/gttvkheoxp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtfppjndah.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gtzqnzvqxg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtfzauwjij.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtdfdthwuh.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gtojfeejht.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258.top/gtzwmdfdas.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hammf.cn/gthdnwdbih.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtzitlwobt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gticzfuwuo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gtwzkcoeaq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtyawdwcjq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtzavstmtl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtorjwrovj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gttbxcqdog.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtaaxvyvvs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtiajmejsq.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gtakajzvqk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtsfwzoibh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gttxibtacp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtwilxhhoo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtsrbexfyl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtsylwmerp.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtkvqfiayj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gtiaohmdhl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ppjwa.cn/gteofninbz.html

================================================================================
来源：http://hz.yvedp.cn/gtbqqkvpec.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtbfxxcjiw.html

================================================================================
来源：http://hz.dashuyun.cn/gtkdxtcghh.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtzlpokjdu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sufxvd.cn/gtsrcvlctq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtpgqrxqrs.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtwvmazvei.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtrqxkhbam.html


<!-- 参考信息 -->