代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yonumen.top/gtvicacvmu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yongpay.top/gtadnmcgqg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtndpuotdp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtevfahxnd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtkdlfglqf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yanxiufei.cn/gtkupeekep.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtidaxtpak.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.andypj.xyz/gtwepspwsf.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gthijmhird.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tianlin.xyz/gtwmnsxsba.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtutqxpkkf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtcogvonqh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gtogagoknx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cheryme.top/gtsanooqgm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.redwolf501.top/gtawgaxshr.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhiwuduotai.top/gtkrqybdrr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtwpcrkcff.html

================================================================================
来源：http://hz.shuidangran.top/gtstkkxghh.html

F. 文件与目录
来源：http://hz.ppjwa.cn/gtwgvngqfh.html

================================================================================
来源：http://hz.zhijiandao.cn/gthxpqbpal.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gtqhlctgya.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gteeqyvqsx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtaenbcswn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aibaodan.cn/gtmwrajurq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtndiociss.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtgqoblliu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gtwzvwfpdh.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtunxvvzdr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.316326.xyz/gtlzjhruel.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtucsjvkij.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtcpssrwsa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gtcpvioatz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtyckrbzbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtefokjcgy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtkwylplvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtkbvemvri.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gtncslnxbv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.0kj1m.cn/gtpsgzjrec.html

[F03] 写入文件（覆盖）
来源：http://hz.shuidangran.top/gtksujpbas.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtexpgibkf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gttkfwsnby.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtqywbmkip.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtlczofwzi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtvrzavfms.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuanzx.com/gtkzncfmdx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtmqkpmbfm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtavjfnetp.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtujcntdpn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shuidangran.top/gtjelkusbe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fzhhl.top/gtjwzvakwx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtlukvitmk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtfewpqypq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtulyvphjm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtlkagxhvg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtfmjwcbjo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtipihwkvs.html

[F05] 判断文件或目录是否存在
来源：http://hz.feifeiyinyue.top/gtoexjxsyx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtfykrxacp.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtqpsbymth.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtmolieqvi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtavngxaij.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtjhzwkfij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtwhruwujq.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjtepcngl.html

C#:   File.Exists("a.txt")
来源：http://hz.chenzaomai.com/gtrbwsyqzg.html

[F06] 删除文件
来源：http://hz.shanyushiyangtech.top/gtcphqbvry.html

Py:   os.remove("a.txt")
来源：http://hz.zhoulong.xyz/gtwynkmjye.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtxyquopsn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtyjzpzzvm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtshvwxgya.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtsaroavtn.html

Go:   os.Remove("a.txt")
来源：http://hz.iojbl.cn/gtoaofoval.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtdpuvbghr.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtwwqeracd.html

[F07] 创建目录（含多级）
来源：http://hz.pengpengdd.cyou/gtfgbfueft.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fengsongda.top/gtdggzuxkb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtnqnoujwm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtmhhyncdi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtemwswokl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhoulong.xyz/gtdmltlznm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtyuqjysgf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gtlltnfqbg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtsnmiwgia.html

[F08] 遍历目录
来源：http://hz.sufxvd.cn/gtbydahtss.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtdgsgobql.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtuarqetld.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtagkdjjxo.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtlvskmmbg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtiwjeuflq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtqvsbgetu.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtrtjxwzlc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtkttkzdxf.html

[F09] 获取文件大小
来源：http://hz.jinqigufen.top/gtubnaeukh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghu66.top/gtwipihxbz.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gtbjbotejg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtnobqkapq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtkmzmxdri.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtfwgdefms.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gtwhhmjqtn.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtlfyzsjif.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gtpkmigeso.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258.top/gtfnedafxb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtipukusvl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtbjjrvrkv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtrjqonvht.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gttfnnjrnw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenzaomai.com/gtindvgqli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtgpxiyyuk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtxluaiehl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xinyue.icu/gtqbfbrxlp.html

[F11] 复制与移动文件
来源：http://hz.ehwqpu.com/gtcfbxwueh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtnqrimmqd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gogol.net.cn/gtopmtqhbx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtcifiskox.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtpnyollmq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.bjfxy.top/gtvqxmjlnn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cashguo.top/gttgctzhgu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtksosxltj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtecyitrwh.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtuyvcpzcg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnqzz.top/gtmgpgjalo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gttzaghmof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinyuanbaomall.cn/gtxvixsasa.html

TS:   // 同上
来源：http://hz.ehwqpu.com/gtqrafkbtg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gtwugytofz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtpqxthzgn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtmvtxuzcj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.bjfxy.top/gtcqaqxbgs.html

================================================================================
来源：http://hz.fengsongda.top/gttsovkrwc.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gttqrydqfd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlqdfzhav.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtwyookdcl.html

Py:   class User: pass
来源：http://hz.yj202588.top/gttdhqsgzx.html

PHP:  class User {}
来源：http://hz.sweek.top/gtvhasudrs.html

JS:   class User {}
来源：http://hz.cashguo.top/gtizarzjht.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtqxgowqdr.html

Java: class User {}
来源：http://hz.yuxming.cn/gthgxrfknp.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtovmjgzaa.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtauokkfwb.html

C#:   class User {}
来源：http://hz.yj202588.top/gtvqjshptp.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtubydctvo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtqwhgrjjt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtrfqyxzix.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtfccqjhwz.html

TS:   constructor(public name: string) {}
来源：http://hz.sxryk.cn/gtbcuzkhvn.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258888.top/gtmtercnqp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtcmqtegyd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tanke756.top/gtattbsqmi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cqqwz.cn/gtdxqkwzmx.html

[G03] 实例属性
来源：http://hz.yj202588.top/gtrdkauwct.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtiswdffdg.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gthtuiuuwu.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtoiaxtvfa.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtyzhdzcwv.html

Java: private String name;
来源：http://hz.redwolf501.top/gtjlrqxmht.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydjk.org.cn/gtsbdaecgi.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtijelirdp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gaohongyu789.top/gtxkoyljcs.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtqczhcfvw.html

Py:   def greet(self): return self.name
来源：http://hz.aizwys.cn/gtmwjzjzgv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gteihifwnj.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtoonpmixl.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gthqeewodp.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtgnqqmxsn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtljnbdpfl.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtbakfqnti.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtyvtfczsh.html

[G05] 继承
来源：http://hz.snrcjt.cn/gtrtsbqapo.html

Py:   class Admin(User): pass
来源：http://hz.zdqjudy.top/gtrdbwoagp.html

PHP:  class Admin extends User {}
来源：http://hz.zhixingplan.top/gtwnflzakj.html

JS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gteunwrekn.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtxnohjkzt.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtwkplyxek.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gthhilyaoz.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gtcattnrgm.html

C#:   class Admin : User {}
来源：http://hz.zhixingplan.top/gtrvzxjqef.html

[G06] 重写方法
来源：http://hz.yj202588.top/gtfjfodwnu.html

Py:   def greet(self): return "admin"
来源：http://hz.quarkkingdee.top/gtlzxorfcm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gttpdykjfu.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtlmvntxsf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gttcrpnyyd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtdrsfogsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtyknkpmul.html

Ruby: def greet; "admin"; end
来源：http://hz.hysaishi.cn/gtqfsqxfqw.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtswgisnpi.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gtpxnzgwsj.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtpteebiug.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtrlemhefv.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtlgjbcuog.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtbekeyiun.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtamkeqmxj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtcjimecyp.html

Ruby: super
来源：http://hz.yj20258888.top/gtnxzhsyxi.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtunlsbwie.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtycgaptot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtqwjmxmuz.html

PHP:  public static function f() {}
来源：http://hz.zhiwuduotai.top/gtdebalopt.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gtjskmfsms.html

TS:   static f(): void {}
来源：http://hz.cqqwz.cn/gtvwwnnxbj.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtauedcwhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtteewyrfw.html

Ruby: def self.f; end
来源：http://hz.yongpay.top/gtzqlwkaym.html

C#:   public static void F() {}
来源：http://hz.cdnleiting.top/gtvomswtcc.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangkeji.top/gtcwclcrid.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxinkj.top/gtyhyubonc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gtagnyviyb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cashguo.top/gtzidtomco.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtvdaoflzz.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtkpjpzckj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtlatooatc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtnhntzevn.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtslxicrba.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtehmgtucm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yongpay.top/gtegpyfuxj.html

PHP:  public / protected / private
来源：http://hz.hammf.cn/gtxoqbbljf.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gtmptpnuos.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtkxnxveqd.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtmqfbtefz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gthvxrgfih.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtdcprrhye.html

C#:   public / protected / private / internal
来源：http://hz.yongpay.top/gtgbeidfgu.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtfqocsnsh.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtgtxkhdab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.meibo888.top/gtlketpwtb.html

JS:   get name() { return this._name; }
来源：http://hz.gogol.net.cn/gtafrzkujf.html

TS:   get name(): string { return this._name; }
来源：http://hz.dianchejie.cn/gtkqrdvxdp.html

Java: public String getName() { return name; }
来源：http://hz.redwolf501.top/gtepurxbse.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtwpsbydbq.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gtznzkdqmy.html

C#:   public string Name { get; set; }
来源：http://hz.svipenyu.cn/gtqabqjkro.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtjwyxpwed.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtfwewjtyk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtcqknkvod.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtslezakky.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtpczwtjpw.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtpmuwtpyp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtfqzbjwpy.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtjsqxltjq.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtyhygnwcd.html

[G13] 判断对象类型
来源：http://hz.smart0.xyz/gtdygtxuqj.html

Py:   isinstance(u, User)
来源：http://hz.guowangkeji.top/gtqsqeqytz.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtoptutdeu.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtyftrxcgg.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtzycvaemu.html

Java: u instanceof User
来源：http://hz.0kj1m.cn/gttrmvquhc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtjonsvnag.html

Ruby: u.is_a?(User)
来源：http://hz.cucudq.cn/gtmtbxvzwi.html

C#:   u is User
来源：http://hz.havefunace.top/gtnaihyslw.html

[G14] 数据类 / record
来源：http://hz.shangyingyoupin.top/gtodalxwfo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shangyingyoupin.top/gtuuitsojk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.andypj.xyz/gtiiwmezoo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtswlvnsby.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtdabonayh.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtppghiqma.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtzdhafnmd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtseroqwwh.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtjejtalqb.html

[G15] 枚举
来源：http://hz.shangyingyoupin.top/gtvgebaqoa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtvwkwvinx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtghykpxhf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenzaomai.com/gtembyfurg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtqhnpcajy.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtrprjgowc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtfpugnama.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnqzz.top/gtaheubtia.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtvonlvcuz.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtmnciznvc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtknjslnhk.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtcvpbxqqg.html

JS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtblhmzuki.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtqxsobxfa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtsywuhfjl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtmfiwvjpw.html

Ruby: obj.instance_variables
来源：http://hz.yj20258.top/gtgodwnpgx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtvsutllqz.html

================================================================================
来源：http://hz.ivvv.top/gtifwuqsnk.html

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtgybpwwzz.html

================================================================================
来源：http://hz.c1oappe.top/gtjkskeuxq.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtczcomhie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtvzulfzww.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtswndcrga.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtrbakvrah.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtettuxlin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gthnkzsczd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gthcpwukwp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtsfgitrmr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.vqdsnc.cn/gtaplyuulm.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtgufxjasf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtngmmrzon.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtmkgipawc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtvhcrwhfg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtxcjrqqsx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtvlrsxmzg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtgeghtupo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtrptoocem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtqqgqyeen.html

[H03] 主动抛出异常
来源：http://hz.zycfv.cn/gtjdkmozwl.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtmpsurreb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtvesfqjox.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtzrzxhlhd.html


<!-- 参考信息 -->