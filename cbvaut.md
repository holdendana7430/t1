代发 wailian999

Go:   if s == "" {}
来源：http://hz.cucudq.cn/gtncucdysw.html

Ruby: if s.empty?
来源：http://hz.ydzc1.top/gtwockxrgp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.kuanghao11.cn/gtunqdtgor.html

[E21] 超长截断加省略号
来源：http://hz.yvedp.cn/gtabwcqgsf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinqigufen.top/gtpacvmyhj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhijiandao.cn/gtgafxqdbd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtbcymofyy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtiqaxgdzd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtfpkojkwx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.316326.xyz/gtxtnbjgmc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtpppykfdn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yangfankeji.com/gtksxxrkcj.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtvcgueduy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shzxlz.cn/gtfokwpnsz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtpsfslgli.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtvpompspe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtdxpylmnl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zycfv.cn/gthgoamran.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtzhhvlcwj.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtchoenapj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pycfn.com/gtbivexezs.html

================================================================================
来源：http://hz.hysaishi.cn/gtrzcsywti.html

F. 文件与目录
来源：http://hz.yj20258888.top/gtapsuuxze.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdytqoxbe.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gtfbfpxfom.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtylmrpplh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtjplguyml.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cheryme.top/gtfefrqhkh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.smart0.xyz/gtutssjqyt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtonvrzkjy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gtycagulrc.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtboqlyklj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtjhdrbmyg.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtdmyaahkx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtogyvqjsd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangtech.top/gtxffknwuc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtidmgtutn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtazmprohv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gthdlnachm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtcdunpdju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtibfsqvxj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtoatzbxzh.html

[F03] 写入文件（覆盖）
来源：http://hz.52xcode.cn/gtztcpngxx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aibaodan.cn/gtsdxmtgqd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtvqitltfl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtizfndtfy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtqltznhkd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtjtgkklha.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtvonpoxeq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhongyouzk.top/gtoyfdbjib.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtdazywkvi.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtdygzxlpx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtizijibuj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtadkpibmk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtffhbknry.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtwfsqgxse.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtzdbztlin.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinyuanbaomall.cn/gtozzwzhwa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtsvhbgyxo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtnzpflkai.html

[F05] 判断文件或目录是否存在
来源：http://hz.gotoacloud.top/gtpazovgfa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtgzinyimg.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtfftdvkiz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtjmcrlqvo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtviuwvbmc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtvyzvmfmd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtdfjnsanm.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gthxtujnsf.html

C#:   File.Exists("a.txt")
来源：http://hz.xylfe.cn/gtbcqjntnn.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtvmtrdkns.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtwdompfnr.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtkeaxvilg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtfdikdinf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gthuejzxmx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtrculbkmh.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtgkrradkp.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtckgjlixj.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gtcumaacgh.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtlfnsfavr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.9152youxi.cn/gtpvzumczx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxuanxn.top/gtekcakekd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtfklvzkef.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtfsyyjmue.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.redwolf501.top/gtwdsmkazs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtknvscywj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtgiiouwue.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.quarkkingdee.top/gtvedtpbuc.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtmnpssjng.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtxsaduhpx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtbvzbfykg.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtjeoayrpt.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtpgyyviwx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtbviupwmj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtdotxeemp.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtyhtzvttd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tanke756.top/gtbahmazae.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtldoqpkgy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gtvsjcnlwo.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtzftsapux.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtjnwbvgxq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtngtbalpn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtqyvcrcws.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gthberusfr.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtgiryghjo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtwqaplrlg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuanzhike.top/gtvkedsgdj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtrwyuvpif.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtamlpmdxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtztliqicg.html

TS:   path.extname("a.txt")
来源：http://hz.sxryk.cn/gtcyiawcfg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtqwjlusrl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tianlin.xyz/gthjooecvn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtrbsdspwc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yongpay.top/gtfwsenqvs.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtmjgytzaf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gttomvgqda.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtnqelzdol.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtdgrftiga.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtjvmvnvwt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtydqvysba.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gthhqqphzx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtehcansmt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtxfcmsbpi.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtzmdatbvj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sufxvd.cn/gtoefguarb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtdcwfqgqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gtdpowoyfv.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtwohvnrfw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtctwbchig.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ybcxt.top/gtnpkpeijp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtzwftgpkm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtzdrxuzqk.html

================================================================================
来源：http://hz.hysaishi.cn/gtxtzuanao.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtqdxbdrzu.html

================================================================================
来源：http://hz.xziqi.cn/gtikmsrluu.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtvsywgmbm.html

Py:   class User: pass
来源：http://hz.dashuyun.cn/gterqsbhtl.html

PHP:  class User {}
来源：http://hz.jqgfzy.top/gtnbahjiph.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtllfodrsm.html

TS:   class User { name: string = ""; }
来源：http://hz.gotoacloud.top/gtpakelujm.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtrjlgljed.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtqxhriepp.html

Ruby: class User; end
来源：http://hz.c1oappe.top/gttynaycwm.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtjrlyjtrr.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gtzpjtoqds.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gttrwmsenx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guannengcc.top/gtkflcqecq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtwlyjqzmu.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gtixbtlhcr.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtqczyqvqz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtvschsuwp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtmutkzzqn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gtehwitujh.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtgaeaxljv.html

Py:   self.name = "x"
来源：http://hz.cqqwz.cn/gtgtjpziof.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gteaeayiro.html

JS:   this.name = "x";
来源：http://hz.yonumen.top/gtzubyddwh.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtqxdfteme.html

Java: private String name;
来源：http://hz.havefunace.top/gtvfrvvxcc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangshuangyany.cn/gtkuzisipf.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtvevudlll.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.316326.xyz/gtnlgzwiqa.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gteczrewin.html

Py:   def greet(self): return self.name
来源：http://hz.jianghu66.top/gtjocuhdyp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gteposdfel.html

JS:   greet() { return this.name; }
来源：http://hz.pycfn.com/gtceuqnvac.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtylfeebnl.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtjscbkosj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtczgxdjzd.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtdntrkvvj.html

C#:   public string Greet() => Name;
来源：http://hz.guannengcc.top/gtwcrllvhe.html

[G05] 继承
来源：http://hz.mhx1999.top/gtetauzcod.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtzagdiega.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gthfdqzqft.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtgeixcose.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtpcozzwkv.html

Java: class Admin extends User {}
来源：http://hz.bjfxy.top/gteusongap.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gtlbraancw.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtzuiifviw.html

C#:   class Admin : User {}
来源：http://hz.jyoumei.cn/gtiwwqdjng.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtbozklacu.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtvovcgwgt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtajdmaoqj.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtwaehzani.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtsrabybxs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gttjycyudy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hfpthk.cn/gtpwegtgaq.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtqcidlino.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtbaqrcpkd.html

[G07] 调用父类方法
来源：http://hz.shzxlz.cn/gtseflvujh.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtbcqmdxnp.html

PHP:  parent::greet();
来源：http://hz.yj20258888.top/gtgczxlcon.html

JS:   super.greet();
来源：http://hz.gzhubu.top/gtpdufcbsl.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gttiaxqtzc.html

Java: super.greet();
来源：http://hz.zhoulong.xyz/gtuarsbkaf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sysykeji.top/gtdzlhniwt.html

Ruby: super
来源：http://hz.xuanzx.com/gtmrqlcixs.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtmkjrqdds.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtxmylbocw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtwikdqajs.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtspcnooqu.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtbffkfyau.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtmdkxanuv.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtwqzoqwgl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgufenzy.top/gtozralsso.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtvwhlppgi.html

C#:   public static void F() {}
来源：http://hz.sweek.top/gtbdzeggyz.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtjmxfwhfz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gterjnptho.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shangyingyoupin.top/gtsexpswiv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtsegcoasl.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtdlzmvpnu.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gtwsdxnwgn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gttprdawwm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gtqajlgmfz.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gtclhvreoe.html

[G10] 访问控制
来源：http://hz.jinqigufen.top/gthfmkjrau.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtxoqszqok.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gtxtmpfnod.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtfruyabhu.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtroxvxysj.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtmktvljxn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tianlin.xyz/gtyklubfau.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtfsqvbcxl.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtvmnubryy.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtvkqulhbp.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtbykuymmi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtpegxjfsp.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtivyppixy.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gthcxgjlfp.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtnwmzpacf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtpyatquva.html

Ruby: attr_accessor :name
来源：http://hz.316326.xyz/gtyszpuhou.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtvpmgdahx.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangtech.top/gtfvbpdfpu.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtuotjaaqh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtqtgnapru.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtkwnfnxam.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtpbdnwyey.html

Java: @Override public String toString() { return name; }
来源：http://hz.yueranfly.top/gtgpmbvxlq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtugujpsvl.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigufen.top/gtpgwythmx.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtaoocjmzr.html

[G13] 判断对象类型
来源：http://hz.xingfuxueyuan.xyz/gtqmtgzhpk.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gterimsmmj.html

PHP:  $u instanceof User
来源：http://hz.zdqjudy.top/gtlwwqvfge.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gtvjuveuil.html

TS:   u instanceof User
来源：http://hz.xziqi.cn/gthmojnkay.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gthpdfydue.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtgorgbmxx.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtnzwsxupk.html

C#:   u is User
来源：http://hz.zycfv.cn/gtptijqypk.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtkkcgoxdz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtfdluapga.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daria6918.cn/gtvolageui.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtwrbouewb.html

TS:   type User = { name: string; age: number };
来源：http://hz.pengpengdd.cyou/gthkufcbtr.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtjuoiojhi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shuidangran.top/gtgooxzgop.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtfzmwdktn.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtjunhkuqp.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtptzpgxsr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhixingplan.top/gtgrwcmoxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtbvnhbuct.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtxemgkdyz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtxzygvhrq.html

Java: enum Color { RED, GREEN }
来源：http://hz.sweek.top/gttrdecmfl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.0kj1m.cn/gtqgwtkahh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aibaodan.cn/gtbdmcghpd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtxjeyjqmd.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgufenzy.top/gtwvsgmxhc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtrbnikuyk.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtlhtyugyp.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtijamvmkm.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtxpvqkfyd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sxryk.cn/gttieevnqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtztpebepk.html

Ruby: obj.instance_variables
来源：http://hz.zhiwuduotai.top/gthkmtiglo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtmrguqpuu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgicxmdjj.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtyvbcqsjw.html

================================================================================
来源：http://hz.fzhhl.top/gtkopjohhs.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtkejpccui.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgfzy.top/gthfvbdgli.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtpnbwhzox.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gthwcgqmen.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtfdvaxaib.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xziqi.cn/gtbdzoxeqb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhaomingkeji.xyz/gteioogine.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.52xcode.cn/gtlngkpflm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ppjwa.cn/gtlbckphpk.html

[H02] finally / ensure 收尾
来源：http://hz.yuxming.cn/gtirhiyzps.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtfcudmipl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtmmvicyyz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtpwvpjyrv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtcxymgaxd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtpdwcvzcb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fengsongda.top/gtmmahynmb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gttzoqxcxy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gthiaphzan.html


<!-- 参考信息 -->