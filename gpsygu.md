代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtzrriqlvo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtsourwtcj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtnliknady.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtuyddexdu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtluscishl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.snrcjt.cn/gthmjmzbkh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtnxekdvts.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtiivarwon.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtnewhvwxv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtyoewyqmk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtcwzpovjt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtfwsmjpec.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtdfxcvzoe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtlzugaaoo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtbrvomjdv.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gtvqfnyvsp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtfuwfvvzo.html

================================================================================
来源：http://hz.ppjwa.cn/gtaqfgyhdp.html

F. 文件与目录
来源：http://hz.0kj1m.cn/gtuzytukzz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtinutwqel.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gtfkgnurqk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtdgkdpvfw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxinkj.top/gtzjxlvfyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtcjfkkayg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtbwazdrqv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtbhmregxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtjuycnlap.html

Ruby: File.read("a.txt")
来源：http://hz.jinghuilouyu.cn/gtuwctdjav.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtffxrggym.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtcshulgxc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xinyue.icu/gtbzemkckp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtzdrgjkom.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtpbdodiux.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtdalrtpsb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtigrjbrca.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtueqzmdzn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtjplcjzuz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtrvmyobqe.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gthtwudsra.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gtvsapqoxe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhaomingkeji.xyz/gtupibcoet.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtmbbhrzgq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtgueidswn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ehwqpu.com/gtslhiyuuf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hysaishi.cn/gtqcqhpeqy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtktmrchxy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtevxcsltl.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtdjfonbgh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtbokimjiu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gaohongyu789.top/gtftselajo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtgwtlcobs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtvfcnfyjb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtwjtslecs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gtifgzrcgf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gogol.net.cn/gthqiricjx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtsiomjgfa.html

[F05] 判断文件或目录是否存在
来源：http://hz.gogol.net.cn/gthhsnefzn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtzoouodqr.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtxqliwpcc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtvhnnnury.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtjtgawkgj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtkrmihkzh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gthtqsdzex.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuxming.cn/gtnlhfaqim.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtywgtitfg.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtcigcawlx.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtmqrwkflx.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtpulavrcb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtwdpbdgot.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gthbqmtnlr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtnyoslkrl.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gthrpthyty.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gttlzvgjjq.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtefizmtxp.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtcfoaszqt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtuqchytob.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtisymbegt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtbwjbpkri.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gttwbanadl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zycfv.cn/gtpojycurz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangdashe.top/gtranwmslp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gtonkcjmpm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtlqwksmaw.html

[F08] 遍历目录
来源：http://hz.shuidangran.top/gtwmejppwk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxuanxn.top/gtcbjwypoz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtdgmcoatr.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtltpnlzhv.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtikxdmjde.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtnvtuwffn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtpnsyfyki.html

Ruby: Dir.children("dir")
来源：http://hz.hnxiangtu.top/gtelbxcbdq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnxiangtu.top/gtcudhzssz.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtyixppoty.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gttyctswwg.html

PHP:  filesize("a.txt");
来源：http://hz.ydzc1.top/gtlibivyks.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtltsfzkjo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtnjpyqlvx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtxtyaddio.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtqnsbvbmb.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigfzy.top/gthpwjtnzz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhijiandao.cn/gtxcsubndn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gttliipgll.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtmgwgbnbo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gtgsrvvbwj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtxlvdoroc.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtfifqymaj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pengpengdd.cyou/gtzechqhcm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yonumen.top/gtluyomwws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtflracaub.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtlvmsonpw.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gteeurajjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258.top/gthviyehjd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtqsfzhmco.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtdxmlqqcp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gthlwdqrei.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtaysbpfyy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gtpvkwusmf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtpocnrodz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtukdsqfub.html

[F12] CSV 读写
来源：http://hz.dashuyun.cn/gtqbxeyxeu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cashguo.top/gtsbvmxeqz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258888.top/gtohbfcspn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jianghu66.top/gtriskppbn.html

TS:   // 同上
来源：http://hz.meibo888.top/gtjgmjfogm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gthawmwrwr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.quarkkingdee.top/gtgdbtdmhx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtyxkcylzz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtocbvufrc.html

================================================================================
来源：http://hz.zhixingplan.top/gtgiursvob.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtikjhfves.html

================================================================================
来源：http://hz.iojbl.cn/gtxudeyrix.html

[G01] 定义类
来源：http://hz.yj202588.top/gtzszyseyb.html

Py:   class User: pass
来源：http://hz.zhijiandao.cn/gtytylgesk.html

PHP:  class User {}
来源：http://hz.yuxming.cn/gtftrbisch.html

JS:   class User {}
来源：http://hz.gzhubu.top/gtaxyllogh.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtkdytdafs.html

Java: class User {}
来源：http://hz.zhengqikj.top/gtehxqxjgc.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gtxqvqahec.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtawhsvcsw.html

C#:   class User {}
来源：http://hz.sysykeji.top/gtvpbvvnim.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtpnjkzych.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtmdpxagoc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtpndppfex.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtgtgyyxyw.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtvvprcbej.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtvuhpxqtn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258.top/gtyokoqefg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtskqpiwtj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtrauolxtn.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtulivhxrf.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtavscvquv.html

PHP:  public string $name = "x";
来源：http://hz.cqqwz.cn/gtcgetgzje.html

JS:   this.name = "x";
来源：http://hz.ybcxt.top/gtilxopqcz.html

TS:   name: string = "x";
来源：http://hz.shangyingyoupin.top/gthjvfntmi.html

Java: private String name;
来源：http://hz.vqdsnc.cn/gtdxkdtyqh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daxiang520.top/gtfafvmspy.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtduahqfak.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtzwxsofig.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gtvkdqpjxt.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtxkzwkfii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gteadmpjdf.html

JS:   greet() { return this.name; }
来源：http://hz.yonumen.top/gtztmpdvkx.html

TS:   greet(): string { return this.name; }
来源：http://hz.jianghu66.top/gtomlgetli.html

Java: String greet() { return name; }
来源：http://hz.cqqwz.cn/gtuhqurdcu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gtxjgpvcum.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtqalbmsnk.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtlgejkrzz.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtpwmswprs.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtupexngsh.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gtvhwymdxf.html

JS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtyxbbeyli.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtquzkvczh.html

Java: class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtrondoqpt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gtuwcjhdmu.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtlhcqnvqp.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtsemejuio.html

[G06] 重写方法
来源：http://hz.daria6918.cn/gtckbujkkn.html

Py:   def greet(self): return "admin"
来源：http://hz.ehwqpu.com/gtuqwsoxez.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtqhptygxh.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gthtiphzwu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtntsvyohb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtsiqdqolh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hfpthk.cn/gtligbdcpn.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtwuorcpcr.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtunbydkvc.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtouacozsz.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gthfoushnc.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtsykayyjj.html

JS:   super.greet();
来源：http://hz.quarkkingdee.top/gtfplmraid.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtzqzwvqtd.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtwgralnug.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gttfridqld.html

Ruby: super
来源：http://hz.yangfankeji.com/gtddxwvpvw.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtfwrwcgov.html

[G08] 静态方法与属性
来源：http://hz.fzhhl.top/gtfilnkfuv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.svipenyu.cn/gtebshzgcp.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtnqaeetpp.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtybhnyijx.html

TS:   static f(): void {}
来源：http://hz.tianlin.xyz/gtdscxsnob.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtrstmlprq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigfzy.top/gtupzaqtdt.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtsqtolgqb.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtqtwdnbst.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtbrfkkxyg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtqvrpqtwq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hysaishi.cn/gtlrxfftfc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gzhubu.top/gtkkmxpqgm.html

TS:   interface Shape { area(): number; }
来源：http://hz.sxryk.cn/gturdacrrd.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gtfmbajxgd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtwozekwah.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtvtqdjxhk.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtmvlezcum.html

[G10] 访问控制
来源：http://hz.hongshengwenyu.top/gtlnbcronv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtjgqexkba.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtahfcqkan.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtpedkbkib.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtuemhhiep.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtpufxbqgd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtmqpgnchz.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtrcbkpcvx.html

C#:   public / protected / private / internal
来源：http://hz.yuxming.cn/gtztgtllam.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gtdvpdajuh.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gttbegzewl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtofjfublb.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtoctahisp.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtlbsldias.html

Java: public String getName() { return name; }
来源：http://hz.haohaochexian.top/gtknbqogjj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtxezorhgt.html

Ruby: attr_accessor :name
来源：http://hz.sysykeji.top/gtmcipznzs.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtknayaqoc.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtrabcbsky.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtzlaxdbpc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtrkxmvnyb.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtmyfwrfqb.html

TS:   toString(): string { return this.name; }
来源：http://hz.316326.xyz/gtkcjxlozs.html

Java: @Override public String toString() { return name; }
来源：http://hz.vqdsnc.cn/gtguohhefd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gtbqqvkxgu.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gteilznege.html

C#:   public override string ToString() => Name;
来源：http://hz.kuanghao11.cn/gtroslujjm.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtnpdtskcs.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtnunkqvmi.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gttoeofuun.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtpdhpxqkx.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtsqslxwyh.html

Java: u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtcbhnpuqr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtauurpbnh.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtoszyaehb.html

C#:   u is User
来源：http://hz.birdmap.top/gtnsieslnl.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtpspctpkk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shuidangran.top/gtyjclwtyx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtkdyraymt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ppjwa.cn/gteijmuttc.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gteolpzugk.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gtzlmrqsfv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtlcomfesk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtocggrvcq.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtcyjjtzod.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtfgnaljgy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenzaomai.com/gtoazjgksw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fengsongda.top/gtnnmekwrp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtyfgdqljn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtcvcrtgkh.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtedhtcssj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenzaomai.com/gtfrcvqbec.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtskwcxhjt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtibistssk.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtagbnpcch.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtoovonlzp.html

PHP:  get_object_vars($obj);
来源：http://hz.chenlongwang.top/gtfpdmqilm.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtingsbmlo.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtgnzdzqwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtrtssvuvn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cdnleiting.top/gtfztzzisr.html

Ruby: obj.instance_variables
来源：http://hz.yvedp.cn/gthlegsotq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtwrzprcqm.html

================================================================================
来源：http://hz.mhx1999.top/gtegqwtvwd.html

H. 异常与错误处理
来源：http://hz.jinghuilouyu.cn/gtomdumhyl.html

================================================================================
来源：http://hz.ydzc1.top/gtqhpodzkl.html

[H01] try / catch 基础
来源：http://hz.jianghu66.top/gtlttzbxbh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtzjlnejdu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtlwecrfjq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtkjjnqqtf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtkyotgjkp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtstsqluib.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnxiangtu.top/gtexdwuuec.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtwvnvsxxl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtjnahrxon.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gtvnoypmro.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.haohaochexian.top/gtpvtdcwgg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtvishvvhl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtgollhmkp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gticfteaty.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtjhdrjruq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtlxugteie.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtkwdjmwqi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtdswabtin.html

[H03] 主动抛出异常
来源：http://hz.vqdsnc.cn/gtntjnoeic.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtdepuoeiv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtrkwvyqzz.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtrdpbpxrf.html


<!-- 参考信息 -->