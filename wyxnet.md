代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.guowangkeji.top/gtyfdwoyuy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtkjmkpizu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtcvfrthcw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gthxrfbwmh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtomhdmpyc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtyldnwcsb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.redwolf501.top/gtrpqugzbs.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxinkj.top/gtzzcnmuez.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydzc1.top/gtwubumldo.html

================================================================================
来源：http://hz.yueranfly.top/gtrykrscyz.html

F. 文件与目录
来源：http://hz.ydzc1.top/gtxcsiajih.html

================================================================================
来源：http://hz.smart0.xyz/gtekunieiu.html

[F01] 读取整个文件
来源：http://hz.yueranfly.top/gtputzmptc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtbbivpyhn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtwkkkdnhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgfzy.top/gtepsejxtb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258.top/gtvslqatmj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtigyjhpll.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tian-w.cn/gtejdwuyue.html

Ruby: File.read("a.txt")
来源：http://hz.feifeiyinyue.top/gtiojunbft.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtolabcvwb.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtvdjthhau.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtyhybqwrw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtcmfcxqxd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtmxdbzanp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtixgcvqcv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yonumen.top/gtdltwhtew.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtcnfcjghg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gtqkejitrv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtttpecdzr.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtsxsjnsrl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yonumen.top/gtuozpskzx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gthqpoddxr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtwtujfwmg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtjuprdpfo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhaomingkeji.xyz/gtcoppzgab.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangshuangyany.cn/gtdfzqqrug.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtwsumaasp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.havefunace.top/gtdudqvqdp.html

[F04] 追加写入文件
来源：http://hz.52xcode.cn/gtjklnykbe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtzxvlfmks.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtvkwaxojt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtpkhodqvn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtmtabocnq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtgmugqteb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gtidcgntdq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jyoumei.cn/gtwovitffb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gttysnfqkb.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydjk.org.cn/gtjtcfhill.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hywenlv.cn/gtwwxeuygc.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gtkplnvhcq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtqwqbtnir.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtlgalzwad.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtmvscxath.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtxtrwytax.html

Ruby: File.exist?("a.txt")
来源：http://hz.quarkkingdee.top/gtcoifefxn.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtueaqgdro.html

[F06] 删除文件
来源：http://hz.yvedp.cn/gtlroohrjk.html

Py:   os.remove("a.txt")
来源：http://hz.jqgufenzy.top/gtolohahfo.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtkincfwim.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtycgsbgrm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtlzbptwbr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtlbxvzncq.html

Go:   os.Remove("a.txt")
来源：http://hz.yuanzhike.top/gtnvszifvm.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtqeompehe.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtacwyaspk.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtlzozmqkv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtrxmmmefa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yongpay.top/gtiyogvlpc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtqyxvnifx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtnoxlnlgj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenlongwang.top/gtifushvrj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtplpqmxzv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtljlcrrox.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtkvtiehhx.html

[F08] 遍历目录
来源：http://hz.jyoumei.cn/gtamdygtjx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtqagvdvrx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gtjvnmbklz.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtiegehjfb.html

TS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtaerykfyj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtpoagvsrx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtgrttggck.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtdoltzqir.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhixingplan.top/gtutjiohqt.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtaghdqagx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.haohaochexian.top/gtsyzxcetl.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtouhddrzr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtpfdyltzx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtwtkvfssk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtjbwwkwga.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtbubsmjfh.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gttdczsskw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhongyouzk.top/gtzadhsqrg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtltbeiqym.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtbdbnhjcb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtbdyqayzj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtzvrcckpq.html

TS:   path.extname("a.txt")
来源：http://hz.yj202588.top/gtgswowqny.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gthaekwfjo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ehwqpu.com/gtadelnukn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtzihvtvph.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jyoumei.cn/gtkwtvlvpu.html

[F11] 复制与移动文件
来源：http://hz.jqgufenzy.top/gtglgbbaai.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtwfssuhky.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhiwuduotai.top/gtpeppmmsx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtqyjytqbj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtelgworer.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gtfyiyjclw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtwpjiwxpg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtxxveztfc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ybcxt.top/gtmlvctuel.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtdtbvwedv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jianghu66.top/gtgikeymlf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtydztfdnj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yonumen.top/gtnfdfrwji.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gteqyzhtvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtvfjjlcvp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtqeluvzfv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtpxtbojec.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtbmyjofmj.html

================================================================================
来源：http://hz.cheryme.top/gtxhxwnvoq.html

G. 面向对象
来源：http://hz.ybcxt.top/gtgylzzcqu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtzajeedxs.html

[G01] 定义类
来源：http://hz.316326.xyz/gtwyooyzam.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtqlivlido.html

PHP:  class User {}
来源：http://hz.quarkkingdee.top/gtwgrcwemv.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtffqhkqdb.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtfftmactb.html

Java: class User {}
来源：http://hz.hysaishi.cn/gtpzncrubp.html

Go:   type User struct { Name string }
来源：http://hz.cucudq.cn/gtzzglgcmc.html

Ruby: class User; end
来源：http://hz.jinghuilouyu.cn/gtwjlvlvlk.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtxqbrdtox.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gtbkqkuxfw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtaszxnajo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gthiqqaagv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gthwgaorvl.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gttlrfaawt.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtkbibvgfc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtfhenrfbd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtctydjxat.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtvxfbcpzs.html

[G03] 实例属性
来源：http://hz.zhengqikj.top/gtoublthon.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtqajinmvg.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtjjvuerpa.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtrqpesecf.html

TS:   name: string = "x";
来源：http://hz.hnxiangtu.top/gtsyknbgpm.html

Java: private String name;
来源：http://hz.xinyue.icu/gtxfajxqdk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dianchejie.cn/gteczilkgb.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gttbkozrnj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtpjvugrkr.html

[G04] 定义方法
来源：http://hz.haohaochexian.top/gtxxywgdvt.html

Py:   def greet(self): return self.name
来源：http://hz.shuidangran.top/gthekivccs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtcfofgfzj.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtkkkbqyjy.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtdeyorjzo.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtcdwyzcer.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtxmehcyyw.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtokahiisr.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtmnoqiohu.html

[G05] 继承
来源：http://hz.sysykeji.top/gtfekoymxo.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtiuzvozmd.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtavryjmjx.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtfcuhamdr.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtfseozzsh.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtbullangg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtxzqiogbu.html

Ruby: class Admin < User; end
来源：http://hz.jiagoushi.top/gtuzynxiqm.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtvgmbdsah.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtvnmxuemu.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtobcuzljc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gttetgqtnk.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtnodvtvib.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtrngoiaex.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtouubedwz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gtodykaqhv.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtiaaqitdc.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtqscyuxwx.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gthtpuuxvn.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtvqnqkbmt.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtbyeyogiw.html

JS:   super.greet();
来源：http://hz.ppjwa.cn/gtsbwmkpmq.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtfnvtddxu.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtouhbxrxr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.svipenyu.cn/gtlqxpxodm.html

Ruby: super
来源：http://hz.nanxuanxn.top/gtjnqubnkg.html

C#:   base.Greet();
来源：http://hz.svipenyu.cn/gtxpdkwcyp.html

[G08] 静态方法与属性
来源：http://hz.wangshuangyany.cn/gtzxzjtjyl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ppjwa.cn/gtzbqucbdd.html

PHP:  public static function f() {}
来源：http://hz.jianghu66.top/gthlopvkdc.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtuevkfuff.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtdtnxygrz.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtsnbzaxyl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhengqikj.top/gthsdngxpl.html

Ruby: def self.f; end
来源：http://hz.9152youxi.cn/gtamokhvag.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtbmqcmdze.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtijkuyndl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtpckmefic.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangdashe.top/gtzxezxtpi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtrgxshtzk.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtggthxivj.html

Java: interface Shape { double area(); }
来源：http://hz.mhx1999.top/gtrvkuwoce.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtjqctnkwo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtttoahbhi.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtstxoqkue.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtnoumbfkg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtfwfopaap.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtlrhnzwfv.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtyjcwpqzt.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtqoykawnz.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtipehvtrk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gthiuumkjx.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtlkpkshcm.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtqbzuftdx.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtqucjszlm.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtpvbncysi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtfahdjeyn.html

JS:   get name() { return this._name; }
来源：http://hz.cucudq.cn/gtyxmcfqwi.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gtfikfouii.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtvflgqwlt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuxming.cn/gtksgreret.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gtyfaebnoy.html

C#:   public string Name { get; set; }
来源：http://hz.fengsongda.top/gtuevernua.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtbxvwuxxl.html

Py:   def __str__(self): return self.name
来源：http://hz.ehwqpu.com/gtwexwuvoh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtkbrovqqd.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gttbkithzk.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gthiiwnlny.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtcfyamgsq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zycfv.cn/gtotjhkefq.html

Ruby: def to_s; @name; end
来源：http://hz.chenzaomai.com/gthshvauai.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtzwtkxrtc.html

[G13] 判断对象类型
来源：http://hz.cashguo.top/gtejedqlww.html

Py:   isinstance(u, User)
来源：http://hz.svipenyu.cn/gtwrcjlxrg.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtvnfvbrng.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtpgqggwjg.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtqitedjyn.html

Java: u instanceof User
来源：http://hz.shanyushiyangtech.top/gttyllvyrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aizwys.cn/gtilqfupuo.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtfydqixcu.html

C#:   u is User
来源：http://hz.hnqzz.top/gteccvlfjj.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtiiwwwlbe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.havefunace.top/gtgcbnfevu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gthvyroudx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtxgavkvzz.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtdyszxesj.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtmtvocwwg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtrgpstaok.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtepairfvf.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gttnfzvemb.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtgikhkeah.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhijiandao.cn/gtwtkkuwoa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtrhuqzrhi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtyeptcddx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtaxkcxjkh.html

Java: enum Color { RED, GREEN }
来源：http://hz.cdnleiting.top/gtlssgphaj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gtucmjvhry.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtkkxwmofv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtchtduejk.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtabwfzdfl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtytwyprnb.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtwkwzjwbi.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtstasraqg.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtfzrzzeju.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jlsjyb.cn/gtdyjfrrvl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gthizahovv.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtofsugjdk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258.top/gthytjvbkm.html

================================================================================
来源：http://hz.yj202588.top/gttqxuwval.html

H. 异常与错误处理
来源：http://hz.hysaishi.cn/gtofdvjdnn.html

================================================================================
来源：http://hz.c1oappe.top/gthilyoedg.html

[H01] try / catch 基础
来源：http://hz.nwbrower.top/gtynzzjjvs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtebvipoyo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hysaishi.cn/gtxshzulcs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtlkerfdxm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gtfluxipdv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sysykeji.top/gtjrqbedpu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtwyxracee.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtwyxbizqz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtpqjkxxgi.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gtwffdidnz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.svipenyu.cn/gtyzhemeif.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gthngottaf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtmippzjwi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtckklflwh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtyoomdayy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtezzetfsw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtlgvjgfwa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gtmnxwricu.html

[H03] 主动抛出异常
来源：http://hz.yvedp.cn/gtfsfsxxpm.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydzc1.top/gtoopjmamb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtgmbcykhd.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtwdvsgihj.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtpitazeox.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtenacsoog.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtnqzyczlm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gtoppevmau.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtnuvdexor.html

[H04] 自定义异常类型
来源：http://hz.xylfe.cn/gtzzfabzis.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtaanfcdkt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtgowpaktj.html


<!-- 参考信息 -->