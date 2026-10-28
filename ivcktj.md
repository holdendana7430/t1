代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtomkrabur.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jianghu66.top/gtgtozxvah.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gtcvuycvkr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtosjodihw.html

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtvrjcwhuf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtikmotcwa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtzfiqjyyq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtytsfcvfe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtlfhzduel.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtbadeomlu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yonumen.top/gtwbbwyhrd.html

Ruby: s.bytesize;  s.length
来源：http://hz.gotoacloud.top/gtkvsievfc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tian-w.cn/gthpjbalze.html

================================================================================
来源：http://hz.sweek.top/gtpmicrgfr.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gttzxcseus.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvaoomdfi.html

[F01] 读取整个文件
来源：http://hz.yuanzhike.top/gthppqqmbo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gaohongyu789.top/gtwkdsxwbm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuanzx.com/gtbvosohpg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtcoyvpfbe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.meibo888.top/gtmsjrgkjg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gttpzljerz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtncdguuat.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gtiptbldcl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtpjprxggn.html

[F02] 逐行读取文件
来源：http://hz.jianghu66.top/gthiloduwl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ybcxt.top/gtczxgzizx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnxiangtu.top/gteshdjozp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtjlrpmdhb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gttpmrabwa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gttdnmtbyk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gtbvcesoaq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.iojbl.cn/gteznrworx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtckfyapxt.html

[F03] 写入文件（覆盖）
来源：http://hz.nanxuanxn.top/gtcokafsom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pengpengdd.cyou/gtsbjhgwmt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtcsvvrkbj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtqvftzegs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gttgguwnxv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.svipenyu.cn/gtodijipqp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gtqjhzyvol.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtmrqrgjcn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.redwolf501.top/gtdagmyqlw.html

[F04] 追加写入文件
来源：http://hz.ybcxt.top/gtfifzxrmm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtvmrrvzux.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtkcvrifvz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtqcwxuojf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtnujntnpl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.kuanghao11.cn/gtqezsdchl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtpekaxcmr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtcpwrmjnr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtunbygobp.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gtgbvezvnr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtgiyabyce.html

PHP:  file_exists("a.txt");
来源：http://hz.guowangkeji.top/gtoyuapkxh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtpkdgwsyr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtnsrmpkyb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtqoogkkyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtyaimyhrz.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtqtkxpdrt.html

C#:   File.Exists("a.txt")
来源：http://hz.tianlin.xyz/gtzpvjlxkj.html

[F06] 删除文件
来源：http://hz.cheryme.top/gtoooayfui.html

Py:   os.remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtcgikjpjs.html

PHP:  unlink("a.txt");
来源：http://hz.yuanzhike.top/gtmifoqvxc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtpfpwtvel.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtmuegqbed.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtymtsnpmo.html

Go:   os.Remove("a.txt")
来源：http://hz.zycfv.cn/gtpaxxjeow.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtpdixwzme.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtoddmlxwu.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtlthaauaj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtkadgvrjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtopfhsehf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtuzvftdit.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtwfahiijd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gthmxcxese.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aibaodan.cn/gtwaquctpu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtjxutttak.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shzxlz.cn/gtcgbkrgfk.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtmirdzkfz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtaftgvkow.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangkeji.top/gtwwyceetk.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtyvyafnra.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gticplyhez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtmxtdmkbo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtmqxpsjhd.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtwzmdzpdv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtaixvzned.html

[F09] 获取文件大小
来源：http://hz.nanxuanxn.top/gtzwstwrfl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.andypj.xyz/gthtgkimcb.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtteoptxgb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtbhsyexlx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gthuedrzqg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtkowczthr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.snrcjt.cn/gtrgzqcfqs.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtpebjpmqq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgfzy.top/gtyfbaxtvj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtisuaanvw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtvwzxwdgg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtffruntfu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtyynikppi.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gtrsnsvsjr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.svipenyu.cn/gtizscbahx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gttrhwsyav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtwzrfvfsy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtdizhlmug.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtayfaunpg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gttajpgfwj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtcbjndbny.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gthfkvkfkz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gthnqcatma.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtecrweyfj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtypsoxozh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtnudujtwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gtojbzdjde.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtlnzidjab.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dianchejie.cn/gtweymynkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtwavxqvjz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtlsvdmagl.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtwxvhbxtr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gtqwmpmemc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtpmozghow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtozunubog.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtiyngwgtz.html

================================================================================
来源：http://hz.xylfe.cn/gtvgzfgkum.html

G. 面向对象
来源：http://hz.jinqigufen.top/gtgftwwhbv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtyyynohin.html

[G01] 定义类
来源：http://hz.yonumen.top/gtzbzqfcaf.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtfvduicso.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gttslxcuyg.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtyqcwalga.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtfnvjgson.html

Java: class User {}
来源：http://hz.c1oappe.top/gtemxmfwfk.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtgvpoydaj.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtootmyzjp.html

C#:   class User {}
来源：http://hz.zhiwuduotai.top/gthyzzxsmm.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gtrnqnmwvw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gzhubu.top/gtkubaeoki.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtoebjxfrp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtuiskzpcu.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtwccapbpb.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtxguumsys.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtjrcpzyzi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtedrfymlr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gtgmebdtdq.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gttohtregp.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtldhjuyox.html

PHP:  public string $name = "x";
来源：http://hz.quarkkingdee.top/gtcwqylylk.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtgdqzglzl.html

TS:   name: string = "x";
来源：http://hz.shzxlz.cn/gttgmxamby.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtgehyujcp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtcvprnnfs.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtfemnkfhq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtlziccwuu.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtzdiguflc.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtmrlrlelc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtwicagzdx.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtduymqwcl.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtrsceaskp.html

Java: String greet() { return name; }
来源：http://hz.ydzc1.top/gtsvplzbot.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xziqi.cn/gtnfukcrbn.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtynxaetrn.html

C#:   public string Greet() => Name;
来源：http://hz.ydzc1.top/gtddqjerbe.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtvnnjsrwx.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtapsnkjot.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtghnfdbvs.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtwmambmtu.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtqkatnlge.html

Java: class Admin extends User {}
来源：http://hz.sweek.top/gtbrmifmku.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtkiiclmkq.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtfeoqmeqo.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtuoaypqfd.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gttcjglljb.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtmnohfqkq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtiktglkgz.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gttnotskcp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtxhqrejkh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtttbyxpje.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtetnxhxdc.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtlifelxsh.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhaomingkeji.xyz/gtyfwmjhpg.html

[G07] 调用父类方法
来源：http://hz.sweek.top/gtyxelgyep.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gtmrdubecn.html

PHP:  parent::greet();
来源：http://hz.xingfuxueyuan.xyz/gtprzbwzdb.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtyyqxigyl.html

TS:   super.greet();
来源：http://hz.sysykeji.top/gtvgewepga.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtigawvhks.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtdbtgysce.html

Ruby: super
来源：http://hz.gzhubu.top/gtxdowfkrm.html

C#:   base.Greet();
来源：http://hz.zhiwuduotai.top/gtjemepbne.html

[G08] 静态方法与属性
来源：http://hz.yanxiufei.cn/gttnjczvkv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hfpthk.cn/gthhgtzbvi.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtzthurfum.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtmohaonjt.html

TS:   static f(): void {}
来源：http://hz.redwolf501.top/gthljylhqz.html

Java: static void f() {}
来源：http://hz.gzhubu.top/gtqyaplmfo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuanzx.com/gtivmxnbzf.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtjrecjkxb.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtypwjgmgd.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gteicbecyw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gthgpcqlfx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.feifeiyinyue.top/gtzujhahxn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtahkuphxb.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtlgpnfwdj.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtbncezrwk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtuwmficyh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtbkiwihtb.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtwcetncra.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtpdwjkfqu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cqqwz.cn/gtsaiedvuo.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtsocjemzl.html

JS:   #private 字段；其余公开
来源：http://hz.redwolf501.top/gtnawtghfh.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtkhdpvvhj.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtjgwelzud.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtqisjhtoh.html

Ruby: public / protected / private
来源：http://hz.cheryme.top/gtlwkdxcgb.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtlewaxtzu.html

[G11] getter / setter
来源：http://hz.andypj.xyz/gtdhhofpvf.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gteyerpotf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtixydbjoc.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtiesyotna.html

TS:   get name(): string { return this._name; }
来源：http://hz.9152youxi.cn/gtirsyinid.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gthvvfdtni.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gtkjhqyrkx.html

Ruby: attr_accessor :name
来源：http://hz.nanxuanxn.top/gthxurlmts.html

C#:   public string Name { get; set; }
来源：http://hz.shuidangran.top/gtkrygvymt.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gtrzvchonp.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtdufucsyi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtvecewoxv.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtdyhjynsj.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtsgtulavw.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtumflpogh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtqebnnufz.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtfoknerpn.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtwwohojmm.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gttlkuzend.html

Py:   isinstance(u, User)
来源：http://hz.tianlin.xyz/gthmwwtzea.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gtltsetuex.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtvdzymrqo.html

TS:   u instanceof User
来源：http://hz.yongpay.top/gtqgffkrjf.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtrpqkjxco.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtwsgvevau.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtibxmcdti.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtoqxaalmc.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtmjgwnhkv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtvfdhdttq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenlongwang.top/gtwsxqphon.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtmscvqung.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtilzpjaau.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtsyygaeth.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sweek.top/gtlowkclbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtcdyjnkix.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtgibbrdwi.html

[G15] 枚举
来源：http://hz.cheryme.top/gtvjzbbgix.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtcrtxoxfm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zycfv.cn/gtyrhjwxhh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtgxjqdmna.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtvwggvzpv.html

Java: enum Color { RED, GREEN }
来源：http://hz.0kj1m.cn/gtgrlpeyld.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtuiteptqo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtdhmxcxub.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtnnpjtuyy.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtckgelfce.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhaomingkeji.xyz/gtyrwauezw.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtfxioqnpf.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtudklsiod.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gttweqazgk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.birdmap.top/gtvkkakjui.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtteczklzo.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gthotuferc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.svipenyu.cn/gtgtsiypdg.html

================================================================================
来源：http://hz.daxiang520.top/gtoyvfiojw.html

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtsxlfzczl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsfzzdbey.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtltqhjcqk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigfzy.top/gtdrhntmfw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangshuangyany.cn/gtjrfaxbeh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtzeiwsmdp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtenqgvjem.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuanzx.com/gtduqtuczn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydjk.org.cn/gtzqutsvlf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtphnqsqat.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigufen.top/gtbuibawxu.html

[H02] finally / ensure 收尾
来源：http://hz.zhijiandao.cn/gtjjdhrowl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtebdlnkis.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtodotdyon.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtskarxaml.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtfdeprefl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtloevyafj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daxiang520.top/gthwskzbuj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtimcsqbyn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangdashe.top/gtgttmqvgb.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtnkwsaoaw.html

Py:   raise ValueError("错误信息")
来源：http://hz.feifeiyinyue.top/gthrarksrp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtpcrwlylp.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtwqcujuzp.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtfjyptfof.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gticeqgutj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.316326.xyz/gtybrugpbn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtshtocaue.html


<!-- 参考信息 -->