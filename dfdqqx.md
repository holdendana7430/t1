代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtdvnisafd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtrmvrpvlw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jyoumei.cn/gtdsswiipb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtuwtfolny.html

[E22] 字节长度与字符长度
来源：http://hz.hnxiangtu.top/gtztseczgz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtxtdxofui.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtmvulpcjx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtettuidri.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtpxpmgequ.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtefgkcbpe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtfhibaoby.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtwzqmjsmk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhaomingkeji.xyz/gtbezgfmnw.html

================================================================================
来源：http://hz.gzhubu.top/gtrravnrvr.html

F. 文件与目录
来源：http://hz.aizwys.cn/gthccrluat.html

================================================================================
来源：http://hz.jianghu66.top/gtvitnjnou.html

[F01] 读取整个文件
来源：http://hz.pycfn.com/gtiepbbagh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtpymwcxqq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.birdmap.top/gtkxzdshur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtzsjuivuo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gotoacloud.top/gtkenzdzxw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtelwtiasw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtmayfwmte.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtlyfqaiso.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtkxmzdogq.html

[F02] 逐行读取文件
来源：http://hz.yuanzhike.top/gtjelpcrzo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtjsolzpvi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gttnpbwysw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtgqhfcgrr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtfcnrilkc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtzmfmarqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhoulong.xyz/gtsmkejhiz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhengqikj.top/gtpogfyitv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtcsyaomaq.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gttxiijmwr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtehsqulao.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yueranfly.top/gtzrqfmmtj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtzeqxozof.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtgxaghdkz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtdoamcbve.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zdqjudy.top/gtgoqukuzv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gttiiqqlmj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.meibo888.top/gtauyrinpz.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtacykfpno.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtvfkokkid.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gogol.net.cn/gtoiuxkrpx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtinvdvmgq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtcgiwyfmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ppjwa.cn/gtsrgrvtbk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtwjtxdcgd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhaomingkeji.xyz/gtdenwmsld.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuetiantiany.cn/gtagwowfkp.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gtyttqffwz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhiwuduotai.top/gtadrnmucq.html

PHP:  file_exists("a.txt");
来源：http://hz.zdqjudy.top/gtsatnsrcn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gteefdcwpj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtnehoxerw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtnacyrias.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gttfrqqpoc.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gttujwymqh.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtcafhxolk.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtooievuca.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtufhelwdc.html

PHP:  unlink("a.txt");
来源：http://hz.hongshengwenyu.top/gttccbbkad.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtgrfnzfzk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtlcjucpjv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtjnrhtwta.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtlivdhzng.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtqfwmtrbu.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtftpwlpgu.html

[F07] 创建目录（含多级）
来源：http://hz.jinghuilouyu.cn/gteypsqpcn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtasrlmfme.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtiqgvjmbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtukkqcvpb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtfibkixmx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yonumen.top/gtpmsvpjsb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gthnpblgqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.bjfxy.top/gtuyenjxra.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yangfankeji.com/gtjyotojpl.html

[F08] 遍历目录
来源：http://hz.pycfn.com/gtkxpcerlg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtmhimorec.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtiwgyqwit.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtyfnewiql.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtutwaqgmc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtprmemwoc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gttmkcahbz.html

Ruby: Dir.children("dir")
来源：http://hz.yj202588.top/gtesqjnioi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtoslcjlcj.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtuxhplucx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxinkj.top/gtzmboqbmb.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtbhvfeamr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtwqdjicht.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtabojknto.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtrxhgwsid.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtkiuxhvfs.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gtnfdksbcj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtvihgqfwi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtecrdzzzh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtredirooo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtehzxaspx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtbjrospkh.html

TS:   path.extname("a.txt")
来源：http://hz.gotoacloud.top/gtnvjpxwsr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gttnouhfqy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtzkfgshkg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtuhhovrjr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtfselzrea.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtxsiqlkoq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtitasbguv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gtkhiywhzp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtapjejoci.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gteyyymart.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtyftjvxhj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.feifeiyinyue.top/gtrcmefxpb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtukhtlula.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sweek.top/gtinlnzdvb.html

[F12] CSV 读写
来源：http://hz.ppjwa.cn/gteegdunbe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gtcjxnjcfj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ppjwa.cn/gtywxcsasq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtidekyoke.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtaisjwjzo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtmkzgxbel.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtjzmigega.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtfgqtxgud.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pycfn.com/gtufvwrxpr.html

================================================================================
来源：http://hz.cashguo.top/gtqhhgotzb.html

G. 面向对象
来源：http://hz.xinyue.icu/gtyjchnzac.html

================================================================================
来源：http://hz.xziqi.cn/gtijsctvqn.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtigxyqvvg.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtbzrhbqvm.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtwkgckrom.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtdzymqefr.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gtbpodaplb.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtucfnursu.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtqpcfvufa.html

Ruby: class User; end
来源：http://hz.yongpay.top/gtufvouqhf.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtwqnqtzgd.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gtihqkzlum.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtxqmkdnyi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtmrnlchwa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtmwrwrltd.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gtutuooxcv.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtloalqkve.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtynwjdgwo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtnxkweiht.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtnldvaltv.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtkfhsqrih.html

Py:   self.name = "x"
来源：http://hz.jiagoushi.top/gtbldrehud.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtqxvcswik.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtldsvlbfz.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtmayidxgz.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtqwdaivnt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtfrnteyyy.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtausyzpth.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtctxkfgax.html

[G04] 定义方法
来源：http://hz.redwolf501.top/gtuxxvcqjw.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtwlfcorgj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtnafdbave.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtisuhvapp.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtbbdxcwor.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gtsiistjwv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtraycgelh.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtaiqsshsp.html

C#:   public string Greet() => Name;
来源：http://hz.316326.xyz/gtpgimsrsv.html

[G05] 继承
来源：http://hz.shanyushiyangtech.top/gtrleenviv.html

Py:   class Admin(User): pass
来源：http://hz.bjfxy.top/gtgmfbmyzb.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gthfbgkfkj.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtyzzsbpcf.html

TS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtpizbrbst.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtpferewvs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fengsongda.top/gtywwifvgz.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtkufryglu.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtttpeowbz.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtxuqabmva.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtrqsqjzfc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtaidpgrna.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtkeupertj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtuisbzegk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtoohebreg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.birdmap.top/gtpioxnihj.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtibxathsr.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gtmokcmpfu.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtgoeisbvj.html

Py:   super().greet()
来源：http://hz.cdnleiting.top/gtnsgptfsn.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtfpcwqasy.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtelfmsbob.html

TS:   super.greet();
来源：http://hz.yj20258888.top/gtryxvpvtd.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtfuilljsf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ybcxt.top/gtakdqebdn.html

Ruby: super
来源：http://hz.yueranfly.top/gtlxcjclut.html

C#:   base.Greet();
来源：http://hz.yvedp.cn/gtzmvwbpka.html

[G08] 静态方法与属性
来源：http://hz.zycfv.cn/gticnnaevo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtgrlrqdgp.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtvyipnini.html

JS:   static f() {}
来源：http://hz.zdqjudy.top/gtftmbsutv.html

TS:   static f(): void {}
来源：http://hz.zdqjudy.top/gtbeqfnmuu.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtqjnhzgdc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtwsgqrjxf.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtnmaaidiy.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtqvlbrkhf.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtpqspleib.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtykzsdjkl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtxexdxehg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cqqwz.cn/gthrfnpeqp.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtsfnvxail.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtpubhczgw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gtujlmkyyg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ywan-chungtsiang.top/gthubrawnk.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtsvlqvaml.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtosixxwds.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtrinvwdvn.html

PHP:  public / protected / private
来源：http://hz.shzxlz.cn/gtluigyjlt.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtkjpdwqwm.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtcqtbrkby.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtmlgpfwwk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cashguo.top/gtczuplzia.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtxtimbxsi.html

C#:   public / protected / private / internal
来源：http://hz.ppjwa.cn/gtepdeokon.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtllodufcy.html

Py:   @property 与 @x.setter
来源：http://hz.ywan-chungtsiang.top/gtmfaswikf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtdnkhoypu.html

JS:   get name() { return this._name; }
来源：http://hz.meibo888.top/gtxxtopnqt.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtbnqoyner.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtnryvsiob.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtqnornjmg.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtlxogxcbe.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtvanzfeqp.html

[G12] 对象转字符串
来源：http://hz.yanxiufei.cn/gtuhqpnczm.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtvbduhtts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtazoimkjd.html

JS:   toString() { return this.name; }
来源：http://hz.zycfv.cn/gtqkmtzdgp.html

TS:   toString(): string { return this.name; }
来源：http://hz.yvedp.cn/gtwlncgama.html

Java: @Override public String toString() { return name; }
来源：http://hz.haohaochexian.top/gtojthufrm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhixingplan.top/gtjnkdykvk.html

Ruby: def to_s; @name; end
来源：http://hz.sxryk.cn/gtpqceppef.html

C#:   public override string ToString() => Name;
来源：http://hz.vqdsnc.cn/gtmjpaefqm.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtzkdvjcid.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtcozmllcj.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtvetzbufi.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtiiuozecq.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtteumdfxu.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtbvreelrc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtanmglxsi.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtjtusfigv.html

C#:   u is User
来源：http://hz.xylfe.cn/gtspowoajd.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtwblfiwki.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtalctfzxb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtcxtbsttk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gtseobnqhh.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gtfibafsgo.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtpvecpmwv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtqoikkbks.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtyycivwum.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtkdzmtmrg.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtvzrcxcjm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gtgteoldvd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gttetfqgpy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtpzbhkjbm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtwnoghjvk.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtkfrlplob.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gtoyseapzq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sweek.top/gteazwcmmb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtsbhvbyds.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtnbojkssu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtalkzfiti.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtsmhxyzfb.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtnptjlmfa.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtmdrsxmrn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtkrgtnssi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtegemeplt.html

Ruby: obj.instance_variables
来源：http://hz.havefunace.top/gtitecrrdh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtpovoknas.html

================================================================================
来源：http://hz.tian-w.cn/gtefkqtyph.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtbebndwqm.html

================================================================================
来源：http://hz.tian-w.cn/gtdcsalopq.html

[H01] try / catch 基础
来源：http://hz.9152youxi.cn/gtdjycqoov.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtfrunuvvb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cucudq.cn/gtbpijowfl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gttehxniqr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtnzlkmakm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtulqvnugr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtrjxkdont.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtriyncjtp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ppjwa.cn/gtwmybqhhq.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtmfdbrvdr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtauvetald.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtasniqupl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtumirftvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtmgtgeice.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtzofgvkgj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtnmwmznod.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtofyzxrqn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtvkjzxcpw.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtlxihytou.html

Py:   raise ValueError("错误信息")
来源：http://hz.hfpthk.cn/gtdzecxvse.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtjwecusie.html

JS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtcolwuqqg.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtnootnkfk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtdirywajh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtekcbyccy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtytinewsp.html


<!-- 参考信息 -->