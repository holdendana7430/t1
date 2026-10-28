代发 wailian999

Go:   if s == "" {}
来源：http://hz.jlsjyb.cn/gtpxgmegbv.html

Ruby: if s.empty?
来源：http://hz.hysaishi.cn/gtnjbadjwi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigufen.top/gttxsuxsby.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtfbsxjcmz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtxcragnyj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gturjzmqir.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtyezavexu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtergzillq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtxibgvfjg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yanxiufei.cn/gtvpmutahi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtjnwhrzav.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxinkj.top/gtivgezgxs.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtyxvcbksy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtrlwqnftq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtxbteefji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtdojyzqjs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtwbwtlikm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtqfhysbua.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtjxzfhoms.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtsdnjimay.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gteierjwkv.html

================================================================================
来源：http://hz.yueranfly.top/gtgyepilxu.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtpvsjzocu.html

================================================================================
来源：http://hz.birdmap.top/gtegdslnqh.html

[F01] 读取整个文件
来源：http://hz.shzxlz.cn/gtyuuhykzv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.52xcode.cn/gtqpamqaht.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gthynrazbk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtszovvbgk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtdupvwljo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtbjmcngry.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gtjgwjosqk.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtawwwqmoy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtovfqejid.html

[F02] 逐行读取文件
来源：http://hz.ydjk.org.cn/gtxrbgmwzt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuanzhike.top/gtgpyjwkiq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daria6918.cn/gtjciiygob.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtywgjyofn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtweocpogj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gthvsvehhj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtptxokiue.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gtzvjurffv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gthhmphllr.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtdylnemmo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtflhhzvrn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtcixeiagy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gttxmvakyf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtffpjqtfd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtvyxrmojj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.guannengcc.top/gtyhfgzytw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtdybdrvfi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtuwypowhb.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtqqindtrp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhengqikj.top/gtnrbfsftx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtcfzkhafe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtrfwrelev.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtdqzwjppl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtnwkmefat.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtgayndcdk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.316326.xyz/gtrjbrrrtt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtffkivtoh.html

[F05] 判断文件或目录是否存在
来源：http://hz.cheryme.top/gthfhymuox.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtriyyyzwf.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtkziapokg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtetqhiyob.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtrivkikbv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtpmrbhdeq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtunodzbqt.html

Ruby: File.exist?("a.txt")
来源：http://hz.birdmap.top/gttwfhfshs.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtryrbgqjo.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtmkcalrno.html

Py:   os.remove("a.txt")
来源：http://hz.smart0.xyz/gtyecciffs.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtprffxjyv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtngilpjth.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gttzjjozwb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtvnvycweo.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtmwqrtkhx.html

Ruby: File.delete("a.txt")
来源：http://hz.chenlongwang.top/gtscvunlmq.html

C#:   File.Delete("a.txt");
来源：http://hz.kuanghao11.cn/gtrejehlcg.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gttntdqefl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gtyciimzrm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gzhubu.top/gttgvdfaoy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtabdysork.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtftfhxpiw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gttnirooxs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.havefunace.top/gtbgbyaevn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtxpddlmbu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtvpjvhclo.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtflguuggu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yongpay.top/gtgueudlxy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.haohaochexian.top/gtvsbtqdci.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtzqhifttv.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtyadrkzly.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtnixqmcrs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinghuilouyu.cn/gttxxvuwfr.html

Ruby: Dir.children("dir")
来源：http://hz.zhengqikj.top/gtdfvuxxbg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtnfysaaol.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtqbzyvngc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtgwkzjhax.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtejlzkxks.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtbltgpers.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtynzlvlfd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtaezldqyh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtreashniu.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtndgdntda.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ehwqpu.com/gtnkhnsfgn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jyoumei.cn/gtvsdcapav.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtdhphjxlk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtlidktfrm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtypjmgylj.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtfmciohvk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenlongwang.top/gtxuxrbfwk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.snrcjt.cn/gtwrvxbsmw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtutjtejsv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cucudq.cn/gtctufulcj.html

[F11] 复制与移动文件
来源：http://hz.smart0.xyz/gtwglrsqfo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtwlmvnkke.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gogol.net.cn/gtorabgafe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtipvjricy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtebkufnia.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtjmoncuwx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xylfe.cn/gtubwcqwgv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtzsbbskqq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gtmrtonabk.html

[F12] CSV 读写
来源：http://hz.cheryme.top/gtvwxzamjr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.c1oappe.top/gtwzkyvzzm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtraudbyld.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuanzx.com/gtltncsxhq.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtwyfngqgh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtasnnolqi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtqydicazu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtingtrpbi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtjmiyacxe.html

================================================================================
来源：http://hz.gzhubu.top/gtiftosgoz.html

G. 面向对象
来源：http://hz.fzhhl.top/gtwrgaokjc.html

================================================================================
来源：http://hz.aibaodan.cn/gtqrvdvgrj.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtcbkobmzd.html

Py:   class User: pass
来源：http://hz.ydjk.org.cn/gtzkepuoui.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtwjtmrjza.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtdsjnrakg.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtmyvfftwl.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtlebzyyma.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gttvaxxikt.html

Ruby: class User; end
来源：http://hz.yongpay.top/gtvcziiavg.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtjznyjlte.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtypbmxmcx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jyoumei.cn/gtyinmcgdl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.haohaochexian.top/gtscsrubit.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtanwbelyh.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxinkj.top/gtzoqwlsvj.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtbwfqhdaj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guannengcc.top/gtbdyhtpel.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hfpthk.cn/gtghmtdgzj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtpbnpkrqc.html

[G03] 实例属性
来源：http://hz.jqgfzy.top/gtddmgnfmm.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtatggjfgh.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gtbsfphhht.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtvzoldjlo.html

TS:   name: string = "x";
来源：http://hz.0kj1m.cn/gtwnkegrqv.html

Java: private String name;
来源：http://hz.pycfn.com/gtknxscqud.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtiuhdqfet.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtdtwqpmhm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtqbqvryrs.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtaqdpzbbc.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtrafypker.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtrcsdhowt.html

JS:   greet() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtttlcsiob.html

TS:   greet(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtbeaohqjm.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtzfcuflpv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtmqzxtdwh.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtfoehrdes.html

C#:   public string Greet() => Name;
来源：http://hz.yuanzhike.top/gtjserebog.html

[G05] 继承
来源：http://hz.xziqi.cn/gtvpsnhakl.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gtyhvkvcwt.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtortnkbuf.html

JS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtyrlxuxyz.html

TS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtazqdqloj.html

Java: class Admin extends User {}
来源：http://hz.sxryk.cn/gttrvdujme.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtpbyqmiuw.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtoqmvanfl.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtgpwoomou.html

[G06] 重写方法
来源：http://hz.meibo888.top/gtfumlgrof.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtpniuxeaa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtwpgciiey.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtjfgvabur.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtbpredhbr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtdrvkbcnh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtdgaoazhk.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtgqgvzjri.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtikpbgwnj.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtbpeiuywl.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtfmvjwfvs.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtdvyrxpwr.html

JS:   super.greet();
来源：http://hz.yonumen.top/gthhiupznx.html

TS:   super.greet();
来源：http://hz.havefunace.top/gtmvvxmdah.html

Java: super.greet();
来源：http://hz.jianghu66.top/gtluvivumq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtlabhncij.html

Ruby: super
来源：http://hz.sysykeji.top/gtrvekdpav.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gttcbtfjzd.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtmjtikrej.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtvsxzabzy.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtkjvlrbyi.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtxfbexcap.html

TS:   static f(): void {}
来源：http://hz.zhijiandao.cn/gtypjunqli.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtbmdspghn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cashguo.top/gtdecyfwwy.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtfnrwatfz.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtoehmoyrx.html

[G09] 接口 / 抽象类
来源：http://hz.tanke756.top/gtdnqmpjrk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtukmuymox.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtznqgwcdr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gtjadeergb.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtzawzmhqb.html

Java: interface Shape { double area(); }
来源：http://hz.cashguo.top/gtgpcttskz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtxiafeywl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtjdvlbfyy.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtlalyibak.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtbkpypsib.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.meibo888.top/gteraenedu.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtysalnpfm.html

JS:   #private 字段；其余公开
来源：http://hz.redwolf501.top/gtniglnotb.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gthztdfomz.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigfzy.top/gtqrqxdemm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtbgvmcejx.html

Ruby: public / protected / private
来源：http://hz.yongpay.top/gtxzafwmvp.html

C#:   public / protected / private / internal
来源：http://hz.zdqjudy.top/gtxuvdktza.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtvdivwfos.html

Py:   @property 与 @x.setter
来源：http://hz.chenzaomai.com/gtwrvrnisk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yonumen.top/gtdjmkctxs.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtmqpnpklu.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtgnmfqysd.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtqrnmkpea.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtjetlssml.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtogllbvoq.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gthklyamld.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtagsifmnz.html

Py:   def __str__(self): return self.name
来源：http://hz.ehwqpu.com/gtahtxypsr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtpigxbhtk.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtcwzcxwvh.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtayelpqed.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gteubtdvty.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.andypj.xyz/gtkhvucyrd.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gttumwtnda.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gthiohrrbc.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gttywvujxc.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtuufspdnf.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gthonpxevf.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtbbgncmir.html

TS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtyapvzhrf.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtupcuxjbm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtmzzszccr.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gttvqwsymw.html

C#:   u is User
来源：http://hz.fzhhl.top/gtgknxsnza.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gtozfiubtm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtxkwbuulr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtkfklwjoe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gthptjycar.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtwdmziqdo.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtrndkmtoz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.vqdsnc.cn/gtmutgdbfl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtdjlnknvx.html

C#:   record User(string Name, int Age);
来源：http://hz.tianlin.xyz/gtvlbjvpqq.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtvgjpjejs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtqlrbsnqi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtqkxqdoeh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtkkneztck.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtgixfctyn.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtcfentgks.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtcmigowku.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtvmgxgage.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtwfraleuv.html

[G16] 对象转数组 / 字典
来源：http://hz.shuidangran.top/gtixaxjvbt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gttlvhtbgz.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtgshsbivt.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gttlstbufs.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtoycpweti.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.snrcjt.cn/gtxgkstbfk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtbazstokm.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtyglvncbi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtrzfxyfqp.html

================================================================================
来源：http://hz.jqgufenzy.top/gteoaaenpm.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gtftpsepqg.html

================================================================================
来源：http://hz.shuidangran.top/gtvjppkhid.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gtgfhhdjoe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gtggrvmmtw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gtsgopkgta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtyhxxbogq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gteduwwgoe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtlkdxwhzc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtsxqktppa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daxiang520.top/gtwzasbmko.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dianchejie.cn/gtjbswdiam.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gtvvikxika.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xylfe.cn/gtnhijuzwa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtwyojzfmj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtmaqtjbgn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtnbifuepp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gthfdyiheu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinyuanbaomall.cn/gtmrfbleiz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtlrzwzjqq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtzwgmaesa.html


<!-- 参考信息 -->