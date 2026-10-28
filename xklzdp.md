代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtnasrmtgs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gtovdcymzd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtxcplsxsd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shuidangran.top/gtnicqcegs.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtfqvtzeqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenzaomai.com/gtrqendazt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtjqwvjdhq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtlqetnzzx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtqsczimwv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtymooexwg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yueranfly.top/gtcnamrjja.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtiqcvzptv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnxiangtu.top/gttdthxbjw.html

================================================================================
来源：http://hz.cqqwz.cn/gtizlixtnd.html

F. 文件与目录
来源：http://hz.sufxvd.cn/gtwxdfownr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgexoaxtu.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtqpfyqvil.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgfzy.top/gtrilgfdtn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtximojanx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtfoazuhcr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yangfankeji.com/gtmwupnexs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtwhvzdzsc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gtsqbqjiju.html

Ruby: File.read("a.txt")
来源：http://hz.mhx1999.top/gtghyxqqdw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtmcmbgblr.html

[F02] 逐行读取文件
来源：http://hz.jqgfzy.top/gtyflttmdy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hfpthk.cn/gtbuwvusim.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtnhgzwoco.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtdsccsncj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtybbalsrv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtoagscspz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dashuyun.cn/gtrcztqfqy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guannengcc.top/gtmxuqebho.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gtwuqxqwns.html

[F03] 写入文件（覆盖）
来源：http://hz.cdnleiting.top/gtgftvjpkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gtsuvnxfms.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtoezzcuvz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtcphunpzv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtgwhkwcef.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtamhuxrcy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gtwfeduyqa.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xingfuxueyuan.xyz/gtiysbftjm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtbbdsjuic.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtgfmhkwqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhiwuduotai.top/gtwpicaxvq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yongpay.top/gtazazvytw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtiwjlsths.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtlcralzzm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gtkvhyeirg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtcdxnlptk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gaohongyu789.top/gtvrtcujdr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtqdzcambb.html

[F05] 判断文件或目录是否存在
来源：http://hz.zycfv.cn/gtlsoqwpkh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtfnppmwlq.html

PHP:  file_exists("a.txt");
来源：http://hz.yonumen.top/gtjrtccvgs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtlsjzmvdj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtpxoreiie.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtxbskebwu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtiocbftaj.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtkzpxaaks.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtlrxmplba.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtesamneyn.html

Py:   os.remove("a.txt")
来源：http://hz.cqqwz.cn/gtfthsytio.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gtzdmenals.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtwvcqtegx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtweydjdbw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtgulffsyn.html

Go:   os.Remove("a.txt")
来源：http://hz.zycfv.cn/gtdqigutwf.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtqnucjrpz.html

C#:   File.Delete("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtfhkldvai.html

[F07] 创建目录（含多级）
来源：http://hz.jqgfzy.top/gtsuquztzb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtumsxzgns.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258888.top/gtrwmzksdx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtotecrpwm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtvibrrzjl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtdrsoqkuf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtddvoloir.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.9152youxi.cn/gtmoqbljfr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gtmosmotpa.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtcluitisq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtgcyoxhcb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtzywbmorz.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtupuehmwh.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gttewjjqno.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtpyxpietz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtzerlitti.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gtbxvsnvcd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gogol.net.cn/gttbudchlx.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtpeffvuuz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgufenzy.top/gtpbbqrgch.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtmrztdohy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtoqokaygg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gthwaxeato.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtwrhbjpab.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtsextzrgw.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtcmrrekvc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtmvwyrzxb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydzc1.top/gtyjwcndfs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtikoiwygw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangdashe.top/gtpdyeskht.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtcyvedqtp.html

TS:   path.extname("a.txt")
来源：http://hz.0kj1m.cn/gtfceyqlpz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fengsongda.top/gtaauiglmo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtsyyqgllv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtqpjaxzuo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtlltsjdgt.html

[F11] 复制与移动文件
来源：http://hz.feifeiyinyue.top/gtfioaqeaa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtewnsbjwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtkxfkhfsq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtsjxsrtnu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtnkioptal.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtlwqwtasc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtcbtvfodc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gttaoydevi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhixingplan.top/gtzeynumdx.html

[F12] CSV 读写
来源：http://hz.yueranfly.top/gtnubxrwpa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtxnjtxqli.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tian-w.cn/gtrklmqsnx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtaxmfrpje.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gthcjuzjbm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtcbbfinto.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtnqnwjmxc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jiagoushi.top/gttdklzgec.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtzomqkyha.html

================================================================================
来源：http://hz.yongpay.top/gtbaltqzpw.html

G. 面向对象
来源：http://hz.c1oappe.top/gtertixyhy.html

================================================================================
来源：http://hz.hysaishi.cn/gthqomhziq.html

[G01] 定义类
来源：http://hz.daxiang520.top/gtywblitjd.html

Py:   class User: pass
来源：http://hz.wangdashe.top/gtvvjbilnx.html

PHP:  class User {}
来源：http://hz.jqgufenzy.top/gtoayjppvo.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtcrtnqifx.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtokszdolh.html

Java: class User {}
来源：http://hz.ydzc1.top/gtuzavqvnc.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gtvdfmgcyi.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtoyadhpgw.html

C#:   class User {}
来源：http://hz.yj20258888.top/gteqktfnzc.html

[G02] 构造函数
来源：http://hz.xylfe.cn/gtxowuftvl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtiqcgrfmh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yueranfly.top/gthacgefnm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtsbwpnutm.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtrjkipzwy.html

Java: User(String name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtiumvuhdk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shangyingyoupin.top/gtfingjrwn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtjhximqqk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhixingplan.top/gtbhtbawzo.html

[G03] 实例属性
来源：http://hz.ywan-chungtsiang.top/gtcfgjipih.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtjjrxubxv.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gtksgslfmd.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtuasxzero.html

TS:   name: string = "x";
来源：http://hz.xinyue.icu/gttjzpudbl.html

Java: private String name;
来源：http://hz.quarkkingdee.top/gtzlbnhmmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hysaishi.cn/gtsrivjacb.html

Ruby: @name = "x"
来源：http://hz.yuxming.cn/gtcmlrvxwh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtkdwpcptp.html

[G04] 定义方法
来源：http://hz.tanke756.top/gtmiqzaxaw.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gttxprzsyv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gttxrvlqbg.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtnntlezpf.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtlkmmvtsm.html

Java: String greet() { return name; }
来源：http://hz.zhijiandao.cn/gtiwuplmqi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtvzldnqrr.html

Ruby: def greet; @name; end
来源：http://hz.yangfankeji.com/gtycoemtdg.html

C#:   public string Greet() => Name;
来源：http://hz.jlsjyb.cn/gtpzitovoz.html

[G05] 继承
来源：http://hz.fzhhl.top/gtgkxgznvc.html

Py:   class Admin(User): pass
来源：http://hz.sweek.top/gtczxxfwah.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258.top/gtiumqimrj.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtghlubsgt.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtifanamsf.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtplziacko.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gteqwyhsef.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtjrgrjetg.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtkcyiavnx.html

[G06] 重写方法
来源：http://hz.shanyushiyangkeji.top/gtqnnxissk.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtdtxubpnw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtpgkbubsq.html

JS:   greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtkbgglacv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtquducypw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cashguo.top/gtphqlkndz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtvjjainak.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtsgjugatb.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj202588.top/gtonundaqm.html

[G07] 调用父类方法
来源：http://hz.wangdashe.top/gtvnyxttjd.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtgxbcqfjy.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtigqslzof.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtyadwzisl.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtxtevqfhx.html

Java: super.greet();
来源：http://hz.52xcode.cn/gtitdcsajg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gtwxpflmae.html

Ruby: super
来源：http://hz.dianchejie.cn/gtvpxttrit.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gtbiytfdrv.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtaavnqhmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxinkj.top/gtvyixksac.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtwkverwtf.html

JS:   static f() {}
来源：http://hz.yuxming.cn/gtbwmfukwh.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gtnowuxulb.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtgfjyqihx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gtyaiwfdvi.html

Ruby: def self.f; end
来源：http://hz.andypj.xyz/gtxlmcrmst.html

C#:   public static void F() {}
来源：http://hz.smart0.xyz/gtvqidzsdu.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtskjweite.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.316326.xyz/gtjpfersxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ppjwa.cn/gtoesuhnfm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gttaxfjngo.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gttclwkeuz.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gtchblwold.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj202588.top/gtqpbzbsjh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.c1oappe.top/gtmdieudlg.html

C#:   interface IShape { double Area(); }
来源：http://hz.snrcjt.cn/gtzpbxvuow.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtgnipnfdl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtwpmgovkt.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtivzxgxbv.html

JS:   #private 字段；其余公开
来源：http://hz.pengpengdd.cyou/gtezjqgmuj.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtmfyjhbjw.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtkkfdhlno.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gttswndnne.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtamfgjekd.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtybamvwbn.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gtuxytwsus.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtlovmhtzt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtohvuhial.html

JS:   get name() { return this._name; }
来源：http://hz.guannengcc.top/gtqwuczzuq.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtptvugypf.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtjwvcpzcj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtccgijfpp.html

Ruby: attr_accessor :name
来源：http://hz.yonumen.top/gtqkkmekgs.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtygonubhs.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtrrowxabv.html

Py:   def __str__(self): return self.name
来源：http://hz.zhijiandao.cn/gtedilvcfg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtnownolxq.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtxynzczhd.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtosjgaiol.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtwqetjoil.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.birdmap.top/gtkqfjfabe.html

Ruby: def to_s; @name; end
来源：http://hz.aizwys.cn/gtahvdhkcu.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtwszkjduk.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtpnkkpmih.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtooxdtnzp.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtemjcwlxa.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtdrkaupdt.html

TS:   u instanceof User
来源：http://hz.ehwqpu.com/gthgxdduzo.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gtnokoatlw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtkqbjxhbq.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtmacxuvjd.html

C#:   u is User
来源：http://hz.yongpay.top/gtkehcwdmq.html

[G14] 数据类 / record
来源：http://hz.hywenlv.cn/gtugwboten.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtiuvykctl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.mhx1999.top/gthwuvdcso.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtwtfsrffq.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gthpusvhpb.html

Java: record User(String name, int age) {}
来源：http://hz.hfpthk.cn/gtoqsdhzcb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gzhubu.top/gtrztarofq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.0kj1m.cn/gtyrmdblim.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtwuctrnuz.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtrryamonf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.redwolf501.top/gtdguiqzpr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtheaujsty.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtdbgkahbc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtfrosaoco.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtvwmjcpas.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.quarkkingdee.top/gtjaiwjhwx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtdxnvtcmm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtsfadssmq.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtpvvnuewy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gtiyfodstj.html

PHP:  get_object_vars($obj);
来源：http://hz.gzhubu.top/gthbzyvyed.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtdolujbcz.html

TS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gturuaxqah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xingfuxueyuan.xyz/gtfypwlyla.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtomprlttz.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtvcpfetye.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtvfycrbym.html

================================================================================
来源：http://hz.gzhubu.top/gtvykkyqoz.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gtltqzglxe.html

================================================================================
来源：http://hz.bjfxy.top/gteizmqtnn.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gteolqdxfl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtysitgqii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtmrngpcwi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtcmgezidk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtzopewnhm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtabwxmrcy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtnmgaguld.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtnizltkqz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtjtgcjgqo.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtztcvuvhb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gthpvveaud.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gteofpgumk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtwijzzxth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtgmueqcjd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gttxlwkhcx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cdnleiting.top/gtamluufcn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtykqrmuwr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtsrgclfxn.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtpobdoixz.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtjsshlggt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtsjboshhy.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtxroluebt.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtoyyekmcu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtsnauiajc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gotoacloud.top/gtumuwfrsn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj202588.top/gtrzfljtjo.html


<!-- 参考信息 -->