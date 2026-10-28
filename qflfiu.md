代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtfwxjbrgj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xylfe.cn/gtjbdewwrs.html

TS:   if (s === "") {}
来源：http://hz.gotoacloud.top/gtenurxhsw.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtbiefzlnx.html

Go:   if s == "" {}
来源：http://hz.jlsjyb.cn/gtmkulyrcu.html

Ruby: if s.empty?
来源：http://hz.zhixingplan.top/gtbjcfashx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtzhdikspy.html

[E21] 超长截断加省略号
来源：http://hz.gaohongyu789.top/gtkevgupqv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.feifeiyinyue.top/gtapifekvq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gotoacloud.top/gtlhluyesh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtnzsheuge.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtmueqkbyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtubsvkmiy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gthzvgrevf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sufxvd.cn/gtvlpedwwh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aibaodan.cn/gtttkgjtos.html

[E22] 字节长度与字符长度
来源：http://hz.xylfe.cn/gtiuqgseaq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xylfe.cn/gtvxnkhuqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gthijrabvm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gticbibeqc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtkfflwync.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shuidangran.top/gtvuipxcui.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtfdxzmnlt.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhixingplan.top/gtsglnbhyo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinyuanbaomall.cn/gtidypcivw.html

================================================================================
来源：http://hz.jyoumei.cn/gtgjznnjnk.html

F. 文件与目录
来源：http://hz.gzhubu.top/gtrdcpyrko.html

================================================================================
来源：http://hz.andypj.xyz/gtmsiknupr.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtxnjdwppv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.haohaochexian.top/gtnzdexfaj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sweek.top/gtbkpgdexx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cheryme.top/gtqrfvebch.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gtyaohlmlw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gteqesmuyo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ppjwa.cn/gtvfbuxobr.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtsbrvifhp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtnlnqetiy.html

[F02] 逐行读取文件
来源：http://hz.mhx1999.top/gtvvzunwhl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtygdzcaon.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnqzz.top/gtehlhzxkg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtbelltrre.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtjbkamlmg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtgmhiqgrn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pengpengdd.cyou/gtxmbbgvbv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtqanchcwh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jiagoushi.top/gtcfbinpzb.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtcvykedil.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yueranfly.top/gtowpyiquh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtttjatczt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtenquehhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtjgtxzlfp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yangfankeji.com/gtotvjmzvh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtodfdgqih.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.snrcjt.cn/gtdygxbfev.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtrtscmcpi.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtomsyfrzo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtxkpdwlan.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ppjwa.cn/gtcxdvozng.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtvmfjarcj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtijbucrpc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtcibusrrc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtfxiaiwzz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtikqadxpd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gthrghyitb.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gthxmwjivs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258888.top/gthnlxchkh.html

PHP:  file_exists("a.txt");
来源：http://hz.zhixingplan.top/gtxaajiydn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtcuzmpwjs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtgapknyoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtuvgsudcl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtdwyllpuf.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhijiandao.cn/gtzioehlqi.html

C#:   File.Exists("a.txt")
来源：http://hz.cheryme.top/gtafhswvvm.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gttrqggfja.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtdqnznhaf.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtuwrlkjme.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtumodtuya.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtwzvxmrla.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtahbwxiaj.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtosmffzyq.html

Ruby: File.delete("a.txt")
来源：http://hz.gzhubu.top/gtxxbfbfow.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtjgbouvdm.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtvhiadiqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.smart0.xyz/gtdwfzcqlf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yongpay.top/gtgzphdnxe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtprkkurmt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtehkjofgd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtybxhppoo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtarbmcqak.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.316326.xyz/gtzccwotvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtaezphpur.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtjltskybv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtxfcbqsto.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtrewyqkbb.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtlkoszyfd.html

TS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtuxftdzec.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtlpcplorj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jyoumei.cn/gtjhmwpvta.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtmosxrrlc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtzvvboiwr.html

[F09] 获取文件大小
来源：http://hz.haohaochexian.top/gtgmkbhvco.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tanke756.top/gtwahpwlof.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtewqqmuql.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtcuuqrnfm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtldmnfksr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gteiobiwxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gtfxigqhnw.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtrzawcixk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinghuilouyu.cn/gtnpsfdvui.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtzneigpkx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtwlsttcdp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhiwuduotai.top/gtfhkbykuw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gthtuejkze.html

TS:   path.extname("a.txt")
来源：http://hz.gzhubu.top/gtchvyfqog.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aizwys.cn/gtwzpwtihy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sufxvd.cn/gtmmnegyeb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtcfcmgezo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtpdfymttz.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtzxfxyabp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtzvalrjuq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.birdmap.top/gtwiyowahn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtpmsclyhv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtvjgrvoct.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtzcsnbwpf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtecsxaxqr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtuzpyangl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtkzppsgsu.html

[F12] CSV 读写
来源：http://hz.svipenyu.cn/gtxcfnbdgp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinyuanbaomall.cn/gtewjvacqj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtjtmohozw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnxiangtu.top/gtbolifqdf.html

TS:   // 同上
来源：http://hz.ydzc1.top/gtcrimqdky.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangdashe.top/gtbaokayvh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtefflcpus.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cashguo.top/gtrbzypqsv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gttfklboov.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdkhvslcu.html

G. 面向对象
来源：http://hz.sxryk.cn/gtzhsacloa.html

================================================================================
来源：http://hz.sufxvd.cn/gtygvwvslh.html

[G01] 定义类
来源：http://hz.aizwys.cn/gtrghhuaqk.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtbyiekshq.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtvnmtzemq.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtpjihachv.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gtlocujmev.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtayzmodqd.html

Go:   type User struct { Name string }
来源：http://hz.jqgfzy.top/gtlgxgdswy.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gttvixlgbe.html

C#:   class User {}
来源：http://hz.tanke756.top/gtpnvlhzvv.html

[G02] 构造函数
来源：http://hz.hfpthk.cn/gtfidvjnwy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tianlin.xyz/gtqczievug.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinyuanbaomall.cn/gtuznwqesv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtkdrntfmw.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtogahgnxs.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtlgaqidse.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guannengcc.top/gtsbnfdvha.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gthcoutifn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtmbbqheqg.html

[G03] 实例属性
来源：http://hz.jianghu66.top/gtvajwfssu.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtzrtztueu.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtfyacndkg.html

JS:   this.name = "x";
来源：http://hz.ybcxt.top/gtxzjafnfd.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtlodbdwst.html

Java: private String name;
来源：http://hz.svipenyu.cn/gtwhpddbqp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtwpmwbxtu.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtjnrpnmei.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gttjujqpkh.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gtfnfimwyf.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtuwyozswh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtntjgjarl.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtfzlnndhg.html

TS:   greet(): string { return this.name; }
来源：http://hz.daria6918.cn/gtehwzxsqf.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtnomttntm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtxtnqehrf.html

Ruby: def greet; @name; end
来源：http://hz.yongpay.top/gtgoxebisz.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtoxadwlxn.html

[G05] 继承
来源：http://hz.kuanghao11.cn/gtdzmedkds.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtzllwcbow.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtczfpeixd.html

JS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtueypdxtw.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtzvfbizgx.html

Java: class Admin extends User {}
来源：http://hz.guannengcc.top/gtrxzjsqll.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pycfn.com/gtcbfjdobb.html

Ruby: class Admin < User; end
来源：http://hz.yangfankeji.com/gtpkspkapw.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtswumugun.html

[G06] 重写方法
来源：http://hz.zhijiandao.cn/gthybfmlpl.html

Py:   def greet(self): return "admin"
来源：http://hz.nwbrower.top/gteshkrgzh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtgbbokiyq.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtcpoifalg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtjjtijpgo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tanke756.top/gtsnadvjak.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gttyhppqms.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtigntwnns.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtdtedtmna.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtsukwmeup.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtvogpegha.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtgdtitdls.html

JS:   super.greet();
来源：http://hz.nwbrower.top/gtfulxgihr.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtbqrdatuv.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtrvmgtheh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtmttveblm.html

Ruby: super
来源：http://hz.zhijiandao.cn/gttddbmljp.html

C#:   base.Greet();
来源：http://hz.yangfankeji.com/gtkhpopadd.html

[G08] 静态方法与属性
来源：http://hz.yongpay.top/gtwsdyqcbs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hfpthk.cn/gtcevyvbhy.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtmfblychq.html

JS:   static f() {}
来源：http://hz.gogol.net.cn/gtgtmudatr.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtolhbahff.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtxtkagnak.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtentaqnrs.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtocbufsyy.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gtmsnaxsoj.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtbtvhgziz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenlongwang.top/gtqvghyosi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtdqrkrlfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtrkyfvhuf.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gtwbifjghn.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gtqnjjezqe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtxvnerbly.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gthxjdyofr.html

C#:   interface IShape { double Area(); }
来源：http://hz.nanxuanxn.top/gtxrfynyat.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtrpqvibhq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtmlqrdzce.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtdxybxdnv.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtatawgjru.html

TS:   public / protected / private
来源：http://hz.hysaishi.cn/gttdnhbuqu.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtbzlamghj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gttogdpqnp.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtlyubbzzh.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtzhoddpml.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gtuzoiaglv.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtrgalqacd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtzifxcijm.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtrpbzchoi.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtpwxtcbjb.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gtymtbfyra.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtdwbloomd.html

Ruby: attr_accessor :name
来源：http://hz.zhengqikj.top/gtdeabbacx.html

C#:   public string Name { get; set; }
来源：http://hz.cheryme.top/gtszdbfopc.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtlglwabeh.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtcncxaizd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtqkbkgdzp.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtlkzzglgi.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtczzaidst.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinghuilouyu.cn/gtmeunibhy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtcstncpgu.html

Ruby: def to_s; @name; end
来源：http://hz.tianlin.xyz/gtvwfrffgo.html

C#:   public override string ToString() => Name;
来源：http://hz.hnxiangtu.top/gtzxljblsa.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gtkvbctydg.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtcghfonwa.html

PHP:  $u instanceof User
来源：http://hz.cheryme.top/gtcxghpjtd.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtfwbklsbt.html

TS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtsfculyra.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtvvtemgno.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtcbqfbako.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtgnmuvcoj.html

C#:   u is User
来源：http://hz.mhx1999.top/gtqgcnydfe.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtbyhbpjzp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtmizomhqh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gtrtusmgwq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtlbychyqo.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gtsrozljpn.html

Java: record User(String name, int age) {}
来源：http://hz.birdmap.top/gtvwrpktxc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yanxiufei.cn/gtrcgcxpmg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yueranfly.top/gticoqgttp.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtejtozjbm.html

[G15] 枚举
来源：http://hz.yongpay.top/gtaylvlzxz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hywenlv.cn/gtoebynghc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yvedp.cn/gtwkrpzrsx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtpbuqbzsy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtkybsvtuf.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtqyqmlyqv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ywan-chungtsiang.top/gtwbdleeck.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtbmkuupeb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtgdaghblo.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtxoazesix.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtweuqwsmi.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gthrrjffzo.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtlgujjkqp.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtsupddpgm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sysykeji.top/gtmvejsome.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtvpsrtple.html

Ruby: obj.instance_variables
来源：http://hz.cqqwz.cn/gtxgnkexao.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtvcdyssbs.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxhdojthp.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtdlabiixg.html

================================================================================
来源：http://hz.pycfn.com/gtetxrrgpg.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtsparhmbt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtzooyeqxl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtmwhuxfek.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtxucqgqli.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtngljhati.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtxbhddyew.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtczmqnvev.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.52xcode.cn/gtkfjpovky.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gtovpszkdq.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtljhgviyw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtqxanxgbi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtfqdxdtre.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtkotqpimk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtaualpnom.html


<!-- 参考信息 -->