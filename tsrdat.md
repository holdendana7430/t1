代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgfzy.top/gtxqashuet.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtrdlnttzm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtuhrchhct.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ywan-chungtsiang.top/gtypwjdwij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nwbrower.top/gtwkwcbcck.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtqbptsukh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenzaomai.com/gtgpdbkojl.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtxgglvqws.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtuiqmzvlc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gttsswxwyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.mhx1999.top/gtrzyvanoz.html

TS:   // 同上
来源：http://hz.wangdashe.top/gtopensldd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pengpengdd.cyou/gtjnicnvia.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhijiandao.cn/gtbgyryvyb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cqqwz.cn/gtzupyjwxs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xziqi.cn/gtwknnhlof.html

================================================================================
来源：http://hz.bjfxy.top/gtvpuzyvxt.html

G. 面向对象
来源：http://hz.birdmap.top/gtcznegtxy.html

================================================================================
来源：http://hz.xuanzx.com/gtomwlutwe.html

[G01] 定义类
来源：http://hz.shanyushiyangkeji.top/gtyzudknkk.html

Py:   class User: pass
来源：http://hz.zhixingplan.top/gtlyumcsnf.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtdtuugelo.html

JS:   class User {}
来源：http://hz.pycfn.com/gtnywqaraf.html

TS:   class User { name: string = ""; }
来源：http://hz.fengsongda.top/gtagnghbbp.html

Java: class User {}
来源：http://hz.iojbl.cn/gtjqtykweu.html

Go:   type User struct { Name string }
来源：http://hz.wangdashe.top/gtmxecouxl.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtmpgbetgj.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtvirkwnxk.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtbwdqztff.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtcqdkuttu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtersvtpwz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtvqeyrllz.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gthvlhffdv.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtrervjjuz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.quarkkingdee.top/gtvswbjfre.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtquartntk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtbgndwhio.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gtombqbfjf.html

Py:   self.name = "x"
来源：http://hz.xuetiantiany.cn/gtctvtadvq.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtdhjmourn.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtuwtxgeia.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gttvisefhh.html

Java: private String name;
来源：http://hz.jqgufenzy.top/gtwsgdijjo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtlaihnsqa.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtolmsudtz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtklzuqwsy.html

[G04] 定义方法
来源：http://hz.guowangkeji.top/gtsrpkwctl.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtbibtpaqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gthxnsusqa.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtvcrmwega.html

TS:   greet(): string { return this.name; }
来源：http://hz.jianghu66.top/gtzpfsxibl.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtckhztiql.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtjueglyht.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gteqnwsrvg.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtmenihhmr.html

[G05] 继承
来源：http://hz.c1oappe.top/gtqmlqpknn.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gtvakcpsrv.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtdahczcov.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtgohwgktq.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtoirrgwva.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gtzpuhripf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.meibo888.top/gtpwlaghrm.html

Ruby: class Admin < User; end
来源：http://hz.pycfn.com/gtluffrjrz.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtzhrnagqg.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtvpktqhle.html

Py:   def greet(self): return "admin"
来源：http://hz.ppjwa.cn/gtujrhqkdk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtscyenelo.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtsvvdsgfq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtfogwhbxc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258.top/gttdduskst.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgufenzy.top/gtuzoextlb.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtaxmlvnmm.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtfmuotphd.html

[G07] 调用父类方法
来源：http://hz.zhongyouzk.top/gtfmvwhnia.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtpnbxvkap.html

PHP:  parent::greet();
来源：http://hz.sweek.top/gtmuuvasdc.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtnpokqtbk.html

TS:   super.greet();
来源：http://hz.52xcode.cn/gthzhtdydb.html

Java: super.greet();
来源：http://hz.gzhubu.top/gtrwgwsnos.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zycfv.cn/gtkjptjsji.html

Ruby: super
来源：http://hz.316326.xyz/gtdgmcersq.html

C#:   base.Greet();
来源：http://hz.svipenyu.cn/gtqsqkbivi.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtyjfrxfpv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtqnmcfyyd.html

PHP:  public static function f() {}
来源：http://hz.haohaochexian.top/gtdpxqryiw.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtdyfckzzi.html

TS:   static f(): void {}
来源：http://hz.ydzc1.top/gtjmqsnybn.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtuypllgnc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtqxferswi.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gtbcpyjzzb.html

C#:   public static void F() {}
来源：http://hz.wangdashe.top/gtlnfzuqns.html

[G09] 接口 / 抽象类
来源：http://hz.zhaomingkeji.xyz/gtczljtzvb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtmdabzmku.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtqzqrclnu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gtutxpnsqb.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtcmqrezhm.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtrwlyacvd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtgawckvup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtjybvzrnp.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gthyekxeap.html

[G10] 访问控制
来源：http://hz.sufxvd.cn/gtzzzzjosi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtgfwghyjf.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtdpssqvlb.html

JS:   #private 字段；其余公开
来源：http://hz.jqgufenzy.top/gthsgzyajq.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtgcttctks.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtpupjicql.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtarawohgk.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtvqpziilr.html

C#:   public / protected / private / internal
来源：http://hz.jinghuilouyu.cn/gtemtjxwwl.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtfaecdspx.html

Py:   @property 与 @x.setter
来源：http://hz.havefunace.top/gttiuqhdwc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hammf.cn/gtlxjfjlgf.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtkprkbels.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtjufdmidd.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtublrepkk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtkvnobpgf.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtlifxwbjv.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtvixoodsh.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtzqxhhhyw.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtvprudqny.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtbioxondg.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gthwpdgnus.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gtsoaisujm.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnqzz.top/gtbzejshrm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtxofoadki.html

Ruby: def to_s; @name; end
来源：http://hz.xuetiantiany.cn/gtxujrxpnu.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtiynucmsi.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gtpyenfghf.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtjgycyali.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtipjiuzbf.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtssxrvlgq.html

TS:   u instanceof User
来源：http://hz.shuidangran.top/gtwfpuaewi.html

Java: u instanceof User
来源：http://hz.zhixingplan.top/gtdpfmzbty.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.bjfxy.top/gtmkcgkkwe.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtehgfugyk.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtbdcdqnzp.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtwjylmpvk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtltjtcsyy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gthaztgtav.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.kuanghao11.cn/gttlcuitgf.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtdppyaknn.html

Java: record User(String name, int age) {}
来源：http://hz.iojbl.cn/gtudaixpyn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtksfcwozs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gtuwcyzzli.html

C#:   record User(string Name, int Age);
来源：http://hz.9152youxi.cn/gtrqrcijbk.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtsvmfzysn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtjjuckmmc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.haohaochexian.top/gtibzvrmyd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtbhypaaub.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtxjgvoziz.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtsdzrlqrh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuetiantiany.cn/gtivdniidq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtrbimtbzh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtiobxrbop.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtmnjtpqfb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuanzhike.top/gtkokyhyyn.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtsulbkhmc.html

JS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtngrouibe.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtybbwzxgb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigfzy.top/gtkqpfahwu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtledqdcyk.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtaokifuhl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dashuyun.cn/gtrvvkmfft.html

================================================================================
来源：http://hz.mhx1999.top/gtbdsobfux.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtrboictqw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrbljxmbm.html

[H01] try / catch 基础
来源：http://hz.zhengqikj.top/gtpkekzylj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtzmhywawk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtcwnbkhrf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtlnzttdfl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtgfnvoclf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtibqizsds.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtxlorxpvm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtlsvzagri.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtmfitlpkh.html

[H02] finally / ensure 收尾
来源：http://hz.cucudq.cn/gttrrwonqg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtyjcphzaz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtdlbdnhdb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtvaqmnyhr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtwnyknkti.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtbgtlfjfv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtqwxmvmvf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jianghu66.top/gtwfswnmme.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gtaiyierzg.html

[H03] 主动抛出异常
来源：http://hz.zhixingplan.top/gtjfaoabst.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gtenoyiqdc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtfvgyuxua.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtcnssqnrc.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtuxsqyvgp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtqwnwueub.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtywtvlslu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtjhiaothc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtyshwrrug.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gtlcgoctuh.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtsyqcvqfd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gtrjxmcldw.html

JS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtuwybnjqw.html

TS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtkfxiqwei.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtmlekxkhv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shuidangran.top/gtvymhksqh.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtkdirufst.html

C#:   class MyException : Exception {}
来源：http://hz.zhixingplan.top/gtdtdirlna.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtsiqnioxj.html

Py:   except ValueError as e:
来源：http://hz.daria6918.cn/gtxpcycesi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gtfjhtahvd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtxnvwexgq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtcurtmcci.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtbybpzqjl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtavegfzbk.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtalreffcw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gttsrbkzcc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtyvafkqnf.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gtpkrpivcs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtjdlqfmch.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtekwgneja.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtssukhahf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuanzx.com/gtbodbushf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydjk.org.cn/gtykithojk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtvzmwqrvu.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtmliuivlx.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtjaxexfqe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydjk.org.cn/gtkqxdcrcu.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtkubbotob.html

JS:   console.assert(x > 0);
来源：http://hz.jiagoushi.top/gtgmjpockp.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtkqpturdi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtmyivxhlf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtxcbxsamu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xylfe.cn/gtmydpkefk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gtrogcboof.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtsncsvaja.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtpbtzsnlq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtrtvbbgys.html

JS:   e.message;  e.stack
来源：http://hz.pengpengdd.cyou/gtnwqbkolo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtvcdqljoj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtkadtwtdu.html

Go:   err.Error()
来源：http://hz.jianghu66.top/gtydgmlzmz.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtrzcewdxs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtpsntsquk.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtgqcljpyq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtqhddualb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtydztqawr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtbzpaxxvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtzqtgatjt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtvynjcrxh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtywagzeob.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtkgnsyspz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenzaomai.com/gtuwbvirhn.html

[H10] 资源自动释放
来源：http://hz.zhongyouzk.top/gtmyiyxvjn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gtcpnpygal.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtnljnfrew.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtfzywtgye.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtjvdrujdk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gteexozcir.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gthozxfzas.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtdgnlnbpt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtugbcjsbo.html

================================================================================
来源：http://hz.xziqi.cn/gtuddiiaoo.html

I. 正则表达式
来源：http://hz.ppjwa.cn/gtzrxqvxce.html

================================================================================
来源：http://hz.snrcjt.cn/gtdbqdrzev.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gtinaybfhu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtfoyejvei.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtcnqsmueg.html

JS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtkkcmympz.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtaezkeggq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtwhkdlser.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.birdmap.top/gtwtbykohi.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtfzmikbnj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtyjtkerwg.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtpxafslef.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtufiwjvsu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtigoswhxr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cashguo.top/gtlvhubgbi.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtjlfxqsvq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gtafmxnmly.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtmlibczgm.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtgswgwcsw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtnhxklqdv.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtpqphgzml.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gtmacmyviv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gtvvjgalfq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gtykifhjsm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtbbrysoqd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.quarkkingdee.top/gtrcjgvpjq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtsormlfne.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtsbudphoe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtctffqchf.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gtlufosemp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtavvzlkkt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gtcsskwiac.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gthcjbdcxe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtkpsisdkc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtkscisasu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtpbgjczhi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtlueykopl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtaxxjevyc.html

[I05] 按正则拆分
来源：http://hz.fengsongda.top/gtujaamspd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtsyvwndqu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtnhfrnogl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gttbaqptnq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtdzjzoxhw.html


<!-- 参考信息 -->