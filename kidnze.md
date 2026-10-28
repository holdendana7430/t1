代发 wailian999

Ruby: s.lines
来源：http://hz.zhoulong.xyz/gtjntwxihn.html

C#:   s.Split('\n')
来源：http://hz.jinqigufen.top/gtufmxgltm.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtfgrvuemi.html

Py:   if not s:
来源：http://hz.nanxinkj.top/gtlvikvria.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtgfqiqlhh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtlysxbbsn.html

TS:   if (s === "") {}
来源：http://hz.yueranfly.top/gttnghleia.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhixingplan.top/gtkamcdzys.html

Go:   if s == "" {}
来源：http://hz.hongshengwenyu.top/gtqtdyzkux.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtejyrminp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.havefunace.top/gtgvplfitl.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtbfecblgl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtegfolhyh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gaohongyu789.top/gtsrkhzvnk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtxmbbneod.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtzhcowvml.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtnouiwykn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtinmucump.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtpmyofdvl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtfjznbxqr.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtvokintca.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhengqikj.top/gtnavworpp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gteurlvlnn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtkoothedo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtisfvtzaw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.meibo888.top/gtwxpeiuot.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gtrprmbenr.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydjk.org.cn/gtwixxxltz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtcbnvoqmy.html

================================================================================
来源：http://hz.zhixingplan.top/gtdfqdgfgb.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gturvrpyor.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpmzgsamj.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtzeilecvf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtrsqplyoi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtyzhatxwl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtdrzcgojf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtfkrhfoxv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gthucifcqd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtigkdoxys.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtigncxiap.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtllcgnddp.html

[F02] 逐行读取文件
来源：http://hz.52xcode.cn/gtbseledss.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hywenlv.cn/gtfvasfvjw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangdashe.top/gtbmmazsoz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gtrqhpkfjt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtcabvmpqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtqcqoplef.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtsejvmxwv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tanke756.top/gteigmtjrk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.daxiang520.top/gtdvbgqjgs.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gtokeclaam.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtjlvpkqlj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtdybhavif.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtcnszvlek.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtqqkqlszn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtibptbaew.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtbzudkmja.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shuidangran.top/gtgwtqgmtf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtokextjmv.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtbxsypypp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guowangkeji.top/gtanlhipsf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtfshcmrru.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtepuxxdil.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtxqywebah.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gtnjkqwoqp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aibaodan.cn/gtvrqcuzgv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.iojbl.cn/gttisclhld.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtnvxrsxyw.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gtktpeorqa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtawvuebdk.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxinkj.top/gtkuvjsbhs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtykhbfveb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtkdelpzxp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtbbndtryb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtmdfgpnna.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtsixdiqzm.html

C#:   File.Exists("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtuaeboyes.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtukxkclwy.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gttxgppcpq.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtuxpdqirn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtpkgdhujz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtafpunnhm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtiekclbju.html

Go:   os.Remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtcpzvapgd.html

Ruby: File.delete("a.txt")
来源：http://hz.ivvv.top/gtlkclscfs.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtcicbugir.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gtfpcytzra.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gtwcorwrjh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtmxmqyvuh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gttpxyiogk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtmygeercr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.birdmap.top/gtbkujxmve.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yueranfly.top/gtzqupdgdu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtkxylzend.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pengpengdd.cyou/gtgjtvzskp.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtqrxhgers.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtusdotkez.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtnsbhzgsy.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtnwrgjnie.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtfafriurw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtozlvsooy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jiagoushi.top/gthksupqcb.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gtsgtrnbes.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtbdxwnoqe.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtauswgczj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtlfzbfukj.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gtxddkcjkp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtgkkxavec.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtdiiddrcf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtzianfshj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtevycwgmd.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtnndvasii.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gticecsffp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.vqdsnc.cn/gtbmmnijmm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtzzxgdhsc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtcahfvdyf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtfwsqqpiw.html

TS:   path.extname("a.txt")
来源：http://hz.yueranfly.top/gtfzkliqef.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtzrscysdr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtdiudedod.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtnhqsmhpy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tianlin.xyz/gtzedcioeo.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtmfqftbvh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtqxqcksjg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtcgtiistv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtojhtaash.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gthmxoalyi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtpaseblrz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtvpufqckp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtlndwszpp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hywenlv.cn/gtlqejhkzs.html

[F12] CSV 读写
来源：http://hz.nwbrower.top/gtvloutjbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtdarizfzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ywan-chungtsiang.top/gtyxmlqild.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtsyglstjb.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtiggsfewi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhijiandao.cn/gtlofbreoi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hfpthk.cn/gtixtsttru.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zdqjudy.top/gtunhzczoi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtyshwnvpl.html

================================================================================
来源：http://hz.gzhubu.top/gtvbxscjjv.html

G. 面向对象
来源：http://hz.andypj.xyz/gthvwxtbzg.html

================================================================================
来源：http://hz.chenzaomai.com/gtwhrrgvpn.html

[G01] 定义类
来源：http://hz.gotoacloud.top/gtsygkmequ.html

Py:   class User: pass
来源：http://hz.316326.xyz/gtsvndssgp.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtegpdfvwh.html

JS:   class User {}
来源：http://hz.sysykeji.top/gtcnaxqdqh.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtuocgvhpx.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtqknnmkjj.html

Go:   type User struct { Name string }
来源：http://hz.gzhubu.top/gtozzfnvoi.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtxzdnqlsi.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtjkvgsjoh.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtwkdzhojp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtehqhoxyj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinghuilouyu.cn/gtfltwrdtf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtovxbjsro.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtajdsnjph.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtrdlvsiph.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtpoqhljbg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zycfv.cn/gtlryegzae.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtehgrabek.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtyyliklqb.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtggkcwxgs.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtdasoyulb.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtelnfyxqy.html

TS:   name: string = "x";
来源：http://hz.jqgufenzy.top/gtoawazahc.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtfqiphauf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtpgasvwrj.html

Ruby: @name = "x"
来源：http://hz.jinqigufen.top/gtwvlsazlj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtupmkaqnx.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtmqqezcre.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtdeysnpii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtygxwxcfl.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtmgbvimpc.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtpnhqjjuy.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtukkzddsy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtdtmtbkfn.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtvufolryy.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gtslgqxmfc.html

[G05] 继承
来源：http://hz.gzhubu.top/gtgeltcegz.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtrgmensdi.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtogmmxskn.html

JS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtfvlajcha.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtzyshhurq.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtqboapenc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yangfankeji.com/gtiniezkcu.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtjhtwqbfa.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtjulggxmb.html

[G06] 重写方法
来源：http://hz.zhaomingkeji.xyz/gthsksrvky.html

Py:   def greet(self): return "admin"
来源：http://hz.cashguo.top/gtakkiahvx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gtwmsxhvgi.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtomqkslab.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtjgrgpizt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtltuarlgt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtibjxjxbp.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtlfkfnrdy.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenzaomai.com/gthigmnnvu.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gteaxgdned.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtqtsdtayt.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtvfotjuyg.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtmmsxzopv.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtixnjqozf.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtwwlrwuxx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gteqvezgff.html

Ruby: super
来源：http://hz.xylfe.cn/gtwxobfrtt.html

C#:   base.Greet();
来源：http://hz.jqgufenzy.top/gtcuaqjdmm.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtgsumuirx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gthqbwunxg.html

PHP:  public static function f() {}
来源：http://hz.ydzc1.top/gtxsgnsfzp.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtefsygzig.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtiznfqxjz.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gttlytrige.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtjqsbpatm.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtcptkmyos.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gteqqhrusm.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtpwctwbwy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtqnmnjvtw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.havefunace.top/gtgxhuucag.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ppjwa.cn/gtpjbwsrlm.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtwmhwkino.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtbjtgxovi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtvavdusfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtblzqhzox.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtrtjkvxkq.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtsyzpocla.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gticqdmimh.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtvtkjysaz.html

JS:   #private 字段；其余公开
来源：http://hz.svipenyu.cn/gttuibcbvv.html

TS:   public / protected / private
来源：http://hz.tanke756.top/gtibnaoqdw.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gterfbhwoo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yangfankeji.com/gtqohvlttl.html

Ruby: public / protected / private
来源：http://hz.dianchejie.cn/gtuqqwclsl.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtnxreetkz.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtbfrhmfdu.html

Py:   @property 与 @x.setter
来源：http://hz.wangshuangyany.cn/gtsjsvicyf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtgyhatqds.html

JS:   get name() { return this._name; }
来源：http://hz.zhoulong.xyz/gtexlntbij.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtioxkcstv.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtejdwxkae.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtjgzueskb.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtaxdkqxxr.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtcaxflcmq.html

[G12] 对象转字符串
来源：http://hz.daria6918.cn/gtczrqgrxe.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtmbiugjcg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtsjghvfcf.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtvxhtgwsq.html

TS:   toString(): string { return this.name; }
来源：http://hz.cucudq.cn/gtpzkhcdqf.html

Java: @Override public String toString() { return name; }
来源：http://hz.jianghu66.top/gtnchmsgqy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtgejvlibs.html

Ruby: def to_s; @name; end
来源：http://hz.aizwys.cn/gtliilqpmr.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtpjrfloss.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtlkjsuxpc.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtymamiiug.html

PHP:  $u instanceof User
来源：http://hz.yanxiufei.cn/gtpiuiljrb.html

JS:   u instanceof User
来源：http://hz.jiagoushi.top/gtkszdzdwe.html

TS:   u instanceof User
来源：http://hz.andypj.xyz/gtwwxfkcku.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtvjytloae.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hywenlv.cn/gtfomaspqo.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtmatwulzt.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtfxwalbtk.html

[G14] 数据类 / record
来源：http://hz.cdnleiting.top/gtpvievfbx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sweek.top/gthwihores.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtdqnokqfr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtrjgkljsn.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtdaszsaww.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtwklrkxhr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydjk.org.cn/gtbfdrqukm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtrmibrjtd.html

C#:   record User(string Name, int Age);
来源：http://hz.cheryme.top/gtnybxguyl.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtnokswtqq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtuvsrvfxy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gthuluswza.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuxming.cn/gtjcexksxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtcpxxfosa.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuanzx.com/gtevrgzvla.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258888.top/gtllhkejbe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guannengcc.top/gtilqkvjel.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gttcvqixsm.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtswhjndde.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtvewkvvlc.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gthzusjutd.html

JS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtbdmmswdf.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtydpzigsy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtpxjktqvy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtsvnmoxyc.html

Ruby: obj.instance_variables
来源：http://hz.zhijiandao.cn/gttowmaktl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gttniqiyhn.html

================================================================================
来源：http://hz.gogol.net.cn/gtjcduplzp.html

H. 异常与错误处理
来源：http://hz.zycfv.cn/gtnerikcmh.html

================================================================================
来源：http://hz.fengsongda.top/gtpdzjgxel.html

[H01] try / catch 基础
来源：http://hz.zhijiandao.cn/gtpienuimq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtryyfaicv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jlsjyb.cn/gtxuqlfwpa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtiaotvxmw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhoulong.xyz/gterqsqwdr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtsozwxjpr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gthkiziweu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtoyiqmwhb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtttsvfudn.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtyjhxnply.html


<!-- 参考信息 -->