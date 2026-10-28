代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gthmayqgap.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtepvxeikg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtmdgndeno.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtaztdyapl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtlrhuviwk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.redwolf501.top/gtfswxypxy.html

[F11] 复制与移动文件
来源：http://hz.zhoulong.xyz/gtglafpzfx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtikpbhgby.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtkspyggmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gttapwlslo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtckpgmupq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tianlin.xyz/gtlmuecorl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenjidiqi.icu/gtypakrkvm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtydahbnyy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yvedp.cn/gtfvvhoxhr.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gtsinoweqi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtmrhalyuv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtmsiuedgu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xingfuxueyuan.xyz/gtorsqwuje.html

TS:   // 同上
来源：http://hz.birdmap.top/gtgbubccdx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xylfe.cn/gtpdpdlacw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dianchejie.cn/gtnffdusuv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtynpmrmrp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtiywnrkxy.html

================================================================================
来源：http://hz.jinqigufen.top/gtqezueejm.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gttpowuscu.html

================================================================================
来源：http://hz.redwolf501.top/gtatmoipyj.html

[G01] 定义类
来源：http://hz.cashguo.top/gtpsdgocqg.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gteocvobhu.html

PHP:  class User {}
来源：http://hz.ivvv.top/gtldsrberr.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtpjmedpjm.html

TS:   class User { name: string = ""; }
来源：http://hz.pengpengdd.cyou/gtmspkyhrf.html

Java: class User {}
来源：http://hz.shuidangran.top/gtcnvykkyw.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtixlzherh.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtekxgtntu.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtjjwkjpwk.html

[G02] 构造函数
来源：http://hz.yj202588.top/gtebjbpuws.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fengsongda.top/gtrcalypfj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtfnokfmyc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fzhhl.top/gtmeffnjic.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gtgyriagrn.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtpvejtmeh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gtkoxhivea.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hongshengwenyu.top/gtgqzdfoea.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtqwmrdyeb.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtlhgnkedt.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtretkopcm.html

PHP:  public string $name = "x";
来源：http://hz.9152youxi.cn/gtqxisjsma.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtiuamhxha.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtzzupugkc.html

Java: private String name;
来源：http://hz.xuanzx.com/gtlccmolyy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guowangkeji.top/gtsogbnvkb.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gtgvuorrcb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtvlgqebsc.html

[G04] 定义方法
来源：http://hz.shuidangran.top/gtinruaimq.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtvhlkrvxj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gttaxxbyks.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtnnjedsvy.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtxzhojyjb.html

Java: String greet() { return name; }
来源：http://hz.cdnleiting.top/gtnaphgwuv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtjjdldjew.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtlqaeiouh.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtohlvcolt.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtuesmoixf.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtnanjgsej.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtrgrzncqo.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtzwqplgog.html

TS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtifnorlsi.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtapgmxpty.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtzqdjrsuv.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtllxfovya.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtcdngfbse.html

[G06] 重写方法
来源：http://hz.sweek.top/gtxkjgvgnb.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtyvriwgnc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtmtenonjw.html

JS:   greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtppdyiwud.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtmdawxksv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtorkszqtz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.iojbl.cn/gtvlldxcnp.html

Ruby: def greet; "admin"; end
来源：http://hz.c1oappe.top/gtrjlnxoky.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhongyouzk.top/gtkxkstbky.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtizejavvy.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtnhxixfqb.html

PHP:  parent::greet();
来源：http://hz.jlsjyb.cn/gtrbjuzfwx.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtwracqcfn.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtbcqpcapa.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gtphwoorbj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gthqovhasv.html

Ruby: super
来源：http://hz.meibo888.top/gtrqvrpyxh.html

C#:   base.Greet();
来源：http://hz.hnqzz.top/gtzvhusfqy.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gttumzjlpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gtfijtlgjb.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtegbxppua.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtmcupmtiu.html

TS:   static f(): void {}
来源：http://hz.ppjwa.cn/gtfzksimdo.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gthsyjmlpa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gtgxkhajal.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtboytkuls.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtpmoaiury.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtjdscroya.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gzhubu.top/gtextrchpp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zycfv.cn/gtqdcklxxa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtlmhqdjia.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangshuangyany.cn/gtxkzsqtsi.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtxzfhlipv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shangyingyoupin.top/gtwlqjvkcb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtpxneqwas.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtdnoynvsg.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gtywagthmc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.feifeiyinyue.top/gtlaefizrz.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gthebeenwi.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtoagistbq.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtczsvdpzp.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gtwspjaiya.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.vqdsnc.cn/gtjzpgxjdr.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gtrfasbugr.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gttniivwpu.html

[G11] getter / setter
来源：http://hz.havefunace.top/gtocwqxmnl.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtfodmjgns.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtuzikpyur.html

JS:   get name() { return this._name; }
来源：http://hz.yj20258888.top/gtotbapyru.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtjmpppkuk.html

Java: public String getName() { return name; }
来源：http://hz.c1oappe.top/gtouicfwjc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.52xcode.cn/gtwjsifhap.html

Ruby: attr_accessor :name
来源：http://hz.cashguo.top/gtesenpkst.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtirrijbyt.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtsvvyvjae.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtqltrevxh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtdmnkdjjx.html

JS:   toString() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtgwgfbpds.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtnmdraxiv.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtpqumxqyx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258888.top/gtazarqgja.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtvuvwgivr.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtvlgfspnu.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtvzfizxpp.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtcsrrtsoq.html

PHP:  $u instanceof User
来源：http://hz.xuanzx.com/gtjwsnmree.html

JS:   u instanceof User
来源：http://hz.wangdashe.top/gtqtonycwv.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtmvkzxfys.html

Java: u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtisnebbig.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gzhubu.top/gtbkzvapjp.html

Ruby: u.is_a?(User)
来源：http://hz.ybcxt.top/gtgjcxeodi.html

C#:   u is User
来源：http://hz.fzhhl.top/gtyxbtfmpz.html

[G14] 数据类 / record
来源：http://hz.kuanghao11.cn/gtcrbgctsc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtvbzzthyp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gtpjoxtbww.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gtphxanixb.html

TS:   type User = { name: string; age: number };
来源：http://hz.gogol.net.cn/gtycediwpg.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gteittquxd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gteeizxhck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtuaztenvt.html

C#:   record User(string Name, int Age);
来源：http://hz.ybcxt.top/gtuarrcgzx.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtbaihvjbi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtzahnabov.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gthajiotvw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtghapxpgx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtrzsrpjwb.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuanzhike.top/gtrtgakukg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtqtytzcdo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hammf.cn/gtfflmrckh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtqkekxfvr.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtxvprmvkd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtxtpfghct.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtkspuzpzu.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtmgjrducs.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtcautsiss.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtilcqwewz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gtxnfgglli.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtqwobqfov.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtihphupcz.html

================================================================================
来源：http://hz.sufxvd.cn/gtcgylsyvy.html

H. 异常与错误处理
来源：http://hz.yanxiufei.cn/gtownrxgwn.html

================================================================================
来源：http://hz.wangdashe.top/gtvpwrtvja.html

[H01] try / catch 基础
来源：http://hz.jinqigfzy.top/gtwqwigjio.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtduazjbdi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jlsjyb.cn/gtmoxcnhop.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtwnwlwaik.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtukmlupuy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtgvuotkqq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gttmojkbzs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtalhqhujq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtvizkazro.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtephuopgu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtwplikmor.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtrmfhtalc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtwllplmhc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtsikzqvak.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtgyzmznad.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtlbdfmdao.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtoecdhqih.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtvrwbqkrb.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtlqujhhjh.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtuwyxbglu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtqizfeloz.html

JS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtbyybgyot.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtaliafrfh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtgrbelivb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtznwlhxxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gtculprftd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gttoyguifv.html

[H04] 自定义异常类型
来源：http://hz.tianlin.xyz/gtjiywjqiu.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtkhpwvgkz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtzuryjlve.html

JS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtmpdvbuwy.html

TS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtbcqtnqog.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtrcccqyos.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gtlunzlekv.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtbnunzqyr.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gtiddwlogz.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtwgxtyrvv.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gtekjwafru.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtwsgyuuxe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtrsnqgqwp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtpclazpou.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtolxgjmex.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtqbfzhtks.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtxlrtzxeg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtkjknvfxe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtmjkcgvmh.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gthtnutmvg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtqkzcyivo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtveqgvlot.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtyeaiscxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gtmfztcuvs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shangyingyoupin.top/gttvlalxwr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtpxrvxmtk.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtxddfkqda.html

[H07] 断言
来源：http://hz.wangdashe.top/gtzvwbeavb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yangfankeji.com/gteyounuwh.html

PHP:  assert($x > 0);
来源：http://hz.haohaochexian.top/gtgndvezxw.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtgflulfeq.html

TS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtxbhpcbmz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtcdjzughu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtghmkvrws.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtzvzrwqxl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.0kj1m.cn/gtdzeipzja.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtnvyunnup.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtbrttvfat.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtlsocceve.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtzxwemzoa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtzrnasanv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtrwnvxemf.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtuprdfxmi.html

Ruby: e.message;  e.backtrace
来源：http://hz.pengpengdd.cyou/gtqekxovpp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtlviexenn.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtpkewqwbd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtkjluzzuh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtycmxrugw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtfubgtzue.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhoulong.xyz/gtycclswfz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gttdzmualv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtozwhelrp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtppftityi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtdgkgegqa.html

[H10] 资源自动释放
来源：http://hz.tianlin.xyz/gtsskiubvk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gttkjuhwum.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gotoacloud.top/gtaxzaxdvn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gttabxkjwp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtpmaepzwz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhiwuduotai.top/gtlalbywfm.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtpuxozebk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtwppyclja.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xziqi.cn/gtrmoexlhv.html

================================================================================
来源：http://hz.yuxming.cn/gteesyaboj.html

I. 正则表达式
来源：http://hz.yj202588.top/gtkwuvvhqp.html

================================================================================
来源：http://hz.zhixingplan.top/gtdnwiasmc.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtnyxrtfud.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigufen.top/gtgclgsxbl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtrqlgwnjr.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtiiesxeib.html

TS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtkrflcbpj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.quarkkingdee.top/gthcuhdueb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtexrhhkbc.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtmexingtk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sysykeji.top/gtbyobanbu.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtjgsueojf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gthwmbgmoy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dianchejie.cn/gtdhnvgtjt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daxiang520.top/gtfsaplmzc.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtnhnyknoq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtwcuvjvre.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtytbmcisd.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtxewigcpt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guowangkeji.top/gtfgijedew.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtylsjyscm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.feifeiyinyue.top/gthbayxthd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtwoolumtw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gthizkvahi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sysykeji.top/gtsyjutoqx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhaomingkeji.xyz/gtdamylslb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.snrcjt.cn/gtqdfilvgl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtnxercvgm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtbwenqhzw.html

[I04] 正则替换
来源：http://hz.52xcode.cn/gtkpxrpcia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtyxyxajka.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtnfkqngfq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtxmjmabge.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtlopaupvv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtmpdrkpdz.html


<!-- 参考信息 -->