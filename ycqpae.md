代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gttryhgiaf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gzhubu.top/gtfdxsjelj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtsmmkseax.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sufxvd.cn/gtfijdcrar.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtkeardxij.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.feifeiyinyue.top/gtlpasccvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtqxeopjpd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtzskfttcd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtmffgxrpo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.0kj1m.cn/gtuxejtevu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtfhpcblsl.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtmembcebz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pengpengdd.cyou/gtiwmooess.html

================================================================================
来源：http://hz.yuanzhike.top/gtsgeuccpr.html

F. 文件与目录
来源：http://hz.cashguo.top/gtzpmrikst.html

================================================================================
来源：http://hz.jqgfzy.top/gtohbsdunr.html

[F01] 读取整个文件
来源：http://hz.guannengcc.top/gtqbdfritz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtmowcmenx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj202588.top/gtrufjhggw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtkwjdsagn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtfhpyotxa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtgxnffejg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhixingplan.top/gtblxbwekk.html

Ruby: File.read("a.txt")
来源：http://hz.cdnleiting.top/gtgbwowmtk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.mhx1999.top/gtewimwbuh.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtqlggcixs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gtditgxfaf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.vqdsnc.cn/gtakxhwyqn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtwqsxzsqk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtpbzqeojj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtsnmtxzuz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtetscvkfu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgufenzy.top/gtmypqgiyk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gtxjvmdygl.html

[F03] 写入文件（覆盖）
来源：http://hz.hnqzz.top/gtrjlamxxb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtbzgiynfd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhaomingkeji.xyz/gthuskzclp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtvxkdgibw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtngdsphuz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtsiicwuex.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtzumrkmkb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtogtxyfvr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtlujxdzxu.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtqvlkldis.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtgwhfmvkv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cashguo.top/gtnyeqzkpm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtjrcfddbv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtjfqyyrhq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pycfn.com/gtyxigobst.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtkhcsqckg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtrpmakqgp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtigvqxvpc.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtcnwhzolu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fzhhl.top/gtcbwgbgav.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gtgxcucwmo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenlongwang.top/gtjceehujc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtlrgdgbqj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtitcdkzxf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtbsqveajf.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtvsuliipg.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtldanqorl.html

[F06] 删除文件
来源：http://hz.jianghu66.top/gtxmtzyrkq.html

Py:   os.remove("a.txt")
来源：http://hz.gotoacloud.top/gtzsqywedr.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtoxyeyyfk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtruihpzci.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtpbznwjuz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtrestcywp.html

Go:   os.Remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtjgpljupv.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtcyzleryz.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtbeemzjle.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtkjmtwpfj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daria6918.cn/gteooeacfd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtotbbjueh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtdyfvlovg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtofrkralu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtqhnringk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.haohaochexian.top/gteovtwcsh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtsewytvee.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtepczxlsv.html

[F08] 遍历目录
来源：http://hz.zdqjudy.top/gttirxnoor.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yanxiufei.cn/gtrexcfeih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dianchejie.cn/gtdvsukocc.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtuwyxqroc.html

TS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtoaalbvys.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtvcddulbl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtgyowvtip.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gtkgrgoyyj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtllrzvjnx.html

[F09] 获取文件大小
来源：http://hz.dashuyun.cn/gtavlbjwfp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jyoumei.cn/gtzhcviyzl.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtcqzdugdz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtfipujwrc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtprzqqjtk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtttalfjuz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.c1oappe.top/gtbrgjzebg.html

Ruby: File.size("a.txt")
来源：http://hz.ybcxt.top/gthbhozika.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydjk.org.cn/gtjudmckgn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtoyflrzeb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtvongwtpv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gtzmlvyoee.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtbecgxabz.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtnduiduuh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.andypj.xyz/gthacolyoh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.haohaochexian.top/gttseqikpm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtheicvpkl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gtdpdusaeg.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtcbvsuomv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtfdcrbzrg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtsdaadmrd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtflsluxzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtjkoynfzk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fzhhl.top/gtyajeqdzr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.bjfxy.top/gtauypnrph.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtbqpnafcs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtiltimcrj.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gthzcsvqtd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gtxuazewyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtyjeeckns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dianchejie.cn/gtjyzpggwl.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtcpsnqtqb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gtdmganlth.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigufen.top/gtwgfgwiuy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuanzx.com/gtuypagrrf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtbvlwynqe.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyfaekyor.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtwfsmtqyw.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwkkwanou.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtwgmumuot.html

Py:   class User: pass
来源：http://hz.yuanzhike.top/gtcydihgft.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtmnqvfype.html

JS:   class User {}
来源：http://hz.jyoumei.cn/gtvezvjiie.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtzbcliekx.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtbiydqabj.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtzbsrulbn.html

Ruby: class User; end
来源：http://hz.nwbrower.top/gtluduxnzm.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gtccyrqsrw.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gtbnuaefdv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtqnqwyvwy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtwggkwvfu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtnrgvqtah.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtypbitejt.html

Java: User(String name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtqyaxeocm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtokwfsvsf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtyehtatvp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.iojbl.cn/gtlypisnjc.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gtvbcdemcx.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtpusgsljs.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtdlqhojob.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtyqkkfmcl.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gtsbyqsusj.html

Java: private String name;
来源：http://hz.cqqwz.cn/gtcznhxswx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtlxhfmiev.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtogbvaoml.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtscffdnbx.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtupeouvqt.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtebqumzto.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtxltrzicl.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtgwflacob.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtledzmhbi.html

Java: String greet() { return name; }
来源：http://hz.ybcxt.top/gtpugsllxj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtzmddecii.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtojvuawif.html

C#:   public string Greet() => Name;
来源：http://hz.yuxming.cn/gtoxiktgny.html

[G05] 继承
来源：http://hz.cheryme.top/gtqpnnziiw.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtkuwwqskq.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtbrburnkw.html

JS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtcsavjnab.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtjhmgyzeq.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtwltinaga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtmidzkehg.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtyqkjswib.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtdxflqosk.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtiblzthsc.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtbhrvlewu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtrvnjlwrt.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtzvclvcrx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtdqlpgtsy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gthzwfqfcq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtbawrlsgo.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtqobjnjsp.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtyrfogxlz.html

[G07] 调用父类方法
来源：http://hz.zdqjudy.top/gtkniafrdm.html

Py:   super().greet()
来源：http://hz.jyoumei.cn/gtzesfeean.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtectjhvvr.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtojgngewz.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtabujgihu.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtirflnkbp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.andypj.xyz/gtisxgkvwk.html

Ruby: super
来源：http://hz.fengsongda.top/gtubxwtpeb.html

C#:   base.Greet();
来源：http://hz.zhongyouzk.top/gtmfrayjxo.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtmniduher.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtvhqxgmjr.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtnnzovamu.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtvklpbnjy.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtltbowmvy.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtykhljgku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.iojbl.cn/gtlmpqkqwu.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtdpgeojgr.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gtxnglrcps.html

[G09] 接口 / 抽象类
来源：http://hz.yj202588.top/gtnpphcluf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtsizqvhui.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.birdmap.top/gttvizaivk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtdmecgpft.html

TS:   interface Shape { area(): number; }
来源：http://hz.pycfn.com/gthkvtjdxo.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258888.top/gtqwwfwawn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shangyingyoupin.top/gtrobcutvy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gtqnadkllk.html

C#:   interface IShape { double Area(); }
来源：http://hz.ybcxt.top/gtwjsndhsl.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gtjrgyiohn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtyaqynyrt.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtbjumrxka.html

JS:   #private 字段；其余公开
来源：http://hz.gogol.net.cn/gtpimssdwo.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtdsckjvjd.html

Java: public / protected / private / 默认包级
来源：http://hz.zhiwuduotai.top/gtwbecxjas.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sxryk.cn/gtweenhdte.html

Ruby: public / protected / private
来源：http://hz.guowangkeji.top/gtcjbodglg.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtsbeapoga.html

[G11] getter / setter
来源：http://hz.birdmap.top/gtjmjmkvic.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtonwndtos.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtyutqxbtg.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtrxjljsmz.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtbxfijmwh.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtmkpsayva.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtucqutmyx.html

Ruby: attr_accessor :name
来源：http://hz.yj202588.top/gtwsvkypzv.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangtech.top/gtyhgbtdxk.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtxwqojqze.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtjbrkdaty.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtahicrasn.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gtgdcagbdw.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtgiflczqt.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtghpqabbj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtgapzhdsf.html

Ruby: def to_s; @name; end
来源：http://hz.fzhhl.top/gtzlyansib.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtouopchdh.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtrcikksqw.html

Py:   isinstance(u, User)
来源：http://hz.tianlin.xyz/gtdcoadiis.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtgethwbfg.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtjyymqdsx.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtlvhywdml.html

Java: u instanceof User
来源：http://hz.havefunace.top/gtcprptgbo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtvewqogjq.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtuvhbdjkd.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtbdponcjd.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtylgywdsi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtagsopquf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtsczucikw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtfqvcfihi.html

TS:   type User = { name: string; age: number };
来源：http://hz.bjfxy.top/gtqvpzydzj.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtcsxucmta.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtxzkpkpmi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtpmyjgtfo.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtjcqiouhi.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gturfktxxu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtqgyuwrbc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtoqgggxxm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gtyrtomxay.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtcgiertqu.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtqbmwpeds.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtiewsfzql.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtmccfkogz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtsbxewpow.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtlwkrbkkn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtuukipzbo.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gtkqqrtsjd.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtrrlavgjl.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtygztigbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sxryk.cn/gtfgchzesn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtyrublzyz.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtgmyzmbdl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtfmkvmjpm.html

================================================================================
来源：http://hz.meibo888.top/gtljuvnyye.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtwxeobvhy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gttwndfyrd.html

[H01] try / catch 基础
来源：http://hz.ydzc1.top/gtmzwmdoed.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnqzz.top/gtfwmnvyde.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtllapdpvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtqpcpuyfo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtqwmaxoqr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtkjnfmjqd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtdwdwtknw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtgsvegttz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtipqtuhqt.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gtkrbupnev.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangtech.top/gtppyhfszv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtxinqtfpf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtxvftfstb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtgtfckpec.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtxgvfbxuy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yanxiufei.cn/gtqpgdkjeg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtnjkjwxbr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hysaishi.cn/gtvithclku.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtbirewccd.html

Py:   raise ValueError("错误信息")
来源：http://hz.kuanghao11.cn/gtxtghqfrm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtmkhouuyf.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtbldaijcn.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtrxcliikc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gttjvplyzk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtxlceisyp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.snrcjt.cn/gtkgdkhqxg.html


<!-- 参考信息 -->