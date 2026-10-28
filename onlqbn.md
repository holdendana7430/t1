代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtnfyhvwuh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnxiangtu.top/gtjrnwtlik.html

TS:   if (s === "") {}
来源：http://hz.yonumen.top/gtcrxusftc.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtumrfgtrf.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtgipgcxih.html

Ruby: if s.empty?
来源：http://hz.wangdashe.top/gttngrgjkb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtjflsaqmy.html

[E21] 超长截断加省略号
来源：http://hz.316326.xyz/gtlfaqfyus.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dianchejie.cn/gtoakmuheo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ybcxt.top/gttxntaueu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtwflkltis.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtgabgfabx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtmdewwcqh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gtknluikoo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yueranfly.top/gtjrdukspy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtreggvlci.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtphnwvetz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtxhrievtm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtkpniihln.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtektukhch.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtvgccufdk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuetiantiany.cn/gtllolxmar.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtiguvxxvb.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gtxvrwicad.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuanzhike.top/gtbcfnktmq.html

================================================================================
来源：http://hz.yangfankeji.com/gtbgtnknlx.html

F. 文件与目录
来源：http://hz.yvedp.cn/gtzurtifay.html

================================================================================
来源：http://hz.yj202588.top/gtovjqrnif.html

[F01] 读取整个文件
来源：http://hz.hnqzz.top/gthuhscjvd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.vqdsnc.cn/gtafrgxqsa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gteyriativ.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fengsongda.top/gtqrnxocit.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cqqwz.cn/gtpvcdlwwv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtpiooyxla.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtqqhgyrve.html

Ruby: File.read("a.txt")
来源：http://hz.yangfankeji.com/gtxmdepygd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtilfdamdt.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtxohevgfq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnqzz.top/gtplbkwrle.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnqzz.top/gtkrzzzwhq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtyblimoud.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtrfaibjxd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtmpoamlny.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtqepzbgms.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.andypj.xyz/gtchrdqvtu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenzaomai.com/gtggzlcnxx.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gthoozjsmg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtncyvdmxx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtttmouvgo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtdxelhgyf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtunguurtu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtucndatfp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtutvlumzo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtixxjlwxk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gthmmditqc.html

[F04] 追加写入文件
来源：http://hz.hfpthk.cn/gtkpfbacpx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtjaxqewbw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtuxrfhlou.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtkfqnfkjv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yanxiufei.cn/gtwxvrftvu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtzyqzlion.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtnawvqpfq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydzc1.top/gtchnvpnia.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gtnuxursqv.html

[F05] 判断文件或目录是否存在
来源：http://hz.zycfv.cn/gtgkizwfez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gtojvvovnt.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gtgcbvfeim.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtwuqizmth.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtmzgtbocs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtebdgxsgd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hnqzz.top/gtqvxpfrka.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtrylvwhma.html

C#:   File.Exists("a.txt")
来源：http://hz.chenzaomai.com/gtuntrlptr.html

[F06] 删除文件
来源：http://hz.dashuyun.cn/gtblcflvxs.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqxqkndiu.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtjrajhyyc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.c1oappe.top/gtvhhcvahc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtkzphpurp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtfkktsodq.html

Go:   os.Remove("a.txt")
来源：http://hz.yongpay.top/gttvtafjet.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtosvfuiyj.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtioigatcy.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtwrpaarkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.kuanghao11.cn/gtrkagtxnm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenlongwang.top/gttngtzebq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtgjpmdbok.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtgculwipi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gttmmzecmx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtkkzunxmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtcktlqcyx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtbxhabgnd.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtedrodxnd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtkumlqrhf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtnfwhqdea.html

JS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtyaflxfxu.html

TS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtxrnftdvv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtfbjfirvt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.svipenyu.cn/gtlejjgczu.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtdpegsakb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ywan-chungtsiang.top/gtzztzmjlk.html

[F09] 获取文件大小
来源：http://hz.zhongyouzk.top/gtsujsnizb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuxming.cn/gtukjpxwgr.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtcdupyuni.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gthslpdctd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtbkxbxglu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtifgxxekd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtcmqbligj.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gtpbcfrmgs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtogvhwmda.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinghuilouyu.cn/gtdkjdjpks.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtvlzcfxdb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhongyouzk.top/gtmdvqdhxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtypageadp.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtqnstssew.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.bjfxy.top/gtovjpamuq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hammf.cn/gtapkoronx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtrkzwkice.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.0kj1m.cn/gtplwhtuaw.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtjadufrqu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtgvxhfcuw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gotoacloud.top/gtcksawvgm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtnkirniqz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtvplfmnnf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gttelanips.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtqslkgyzt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtxlimhiqj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.quarkkingdee.top/gtufljxeok.html

[F12] CSV 读写
来源：http://hz.zhongyouzk.top/gtiakpfpcs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtmyyynuba.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtupgerfjg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yanxiufei.cn/gtqcsnjbug.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtsrskqsht.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtjhxkrqce.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtdxywbydg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtlptcuube.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pengpengdd.cyou/gtvzgmvkqb.html

================================================================================
来源：http://hz.jianghu66.top/gtzmdmeayd.html

G. 面向对象
来源：http://hz.sufxvd.cn/gthhyczlit.html

================================================================================
来源：http://hz.meibo888.top/gtsxrrxmkc.html

[G01] 定义类
来源：http://hz.wangdashe.top/gtvbyqevkf.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtkcmrhiop.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtjckbzhln.html

JS:   class User {}
来源：http://hz.yvedp.cn/gtibuygccg.html

TS:   class User { name: string = ""; }
来源：http://hz.sxryk.cn/gtriuxtgwq.html

Java: class User {}
来源：http://hz.yuxming.cn/gtpkexotlq.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtkkarsssk.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtzmkwdajb.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtgpgiyxgi.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gtmnknfmdr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtslylaqwi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtiuuxnhcg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtkipoepvn.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtymnqdcxh.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtbthwrgcu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtkxvmldng.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtfgqsqvff.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtvqzdpdza.html

[G03] 实例属性
来源：http://hz.aizwys.cn/gtsmbauxgb.html

Py:   self.name = "x"
来源：http://hz.tanke756.top/gtarbskbzj.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gtunbqkbqk.html

JS:   this.name = "x";
来源：http://hz.yonumen.top/gtqtebxhhd.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gtsehrrgbt.html

Java: private String name;
来源：http://hz.xziqi.cn/gtuqpjlcwt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtnpfxndhe.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtcvdqqjay.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtkeqmlzha.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtqlmkjsnw.html

Py:   def greet(self): return self.name
来源：http://hz.zdqjudy.top/gtvbvwdqlq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtswwxddah.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtlafpvmna.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtouivnoqh.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtvkcdtshg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtjimyhelh.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtjeunogwq.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtixysemvx.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtstyqnksh.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtzdlfybrf.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtwscymcbl.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtzmdahspp.html

TS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtqwdncbwl.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gtwvzpappd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gttgzeqicu.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtihqauoai.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gtuovjlryy.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtgxlzqkbu.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtumeqsqnt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtouykibyv.html

JS:   greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtrlfzgeez.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtpbqgusec.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtxcxxmatt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtssjdespv.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gterpqqcjl.html

C#:   public override string Greet() => "admin";
来源：http://hz.xziqi.cn/gtntmgfrio.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtvtkatvhs.html

Py:   super().greet()
来源：http://hz.jiagoushi.top/gtoadnkyhf.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtjvgdpjia.html

JS:   super.greet();
来源：http://hz.chenzaomai.com/gtiyhwfujp.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtvapjpobj.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtqbzkkrxl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtksizjocw.html

Ruby: super
来源：http://hz.wangdashe.top/gtxxpmgkgf.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtimjozcii.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtgszrhkfo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtymwfygfl.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtbysedbkj.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gttvklzpml.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtytrxawcm.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtdxspkkoa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtnnkncclp.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtdpdgeqnq.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtajxpfiiu.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtcngxcdli.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtyzddtamr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtofwmizdm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtwrxrotbi.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtxazfyzjf.html

Java: interface Shape { double area(); }
来源：http://hz.yangfankeji.com/gtqgziqmdn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gtqvjvouir.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9152youxi.cn/gtpyxkonsv.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtxebmovnf.html

[G10] 访问控制
来源：http://hz.ybcxt.top/gtkoyfbeud.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtilhhbaqy.html

PHP:  public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtqeelokob.html

JS:   #private 字段；其余公开
来源：http://hz.hysaishi.cn/gtyakpfswr.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtdrqrciwg.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtwkzhjftf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.haohaochexian.top/gtdtugdnos.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gttbveqjjt.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtcpnskxrn.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtqovbfgfw.html

Py:   @property 与 @x.setter
来源：http://hz.chenlongwang.top/gtlwjxcnoi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtfuxefxca.html

JS:   get name() { return this._name; }
来源：http://hz.gogol.net.cn/gtaipqtozp.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtrtioqgcs.html

Java: public String getName() { return name; }
来源：http://hz.yonumen.top/gtowyoqfdh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gttzkjkigm.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtworvngdk.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtewqfqqja.html

[G12] 对象转字符串
来源：http://hz.havefunace.top/gtntughwxv.html

Py:   def __str__(self): return self.name
来源：http://hz.svipenyu.cn/gtvyuxcgdn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtzmlncvrx.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtiwhnxixe.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtxxdharkj.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtvatiwomf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtarmfovwq.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtnpkkojku.html

C#:   public override string ToString() => Name;
来源：http://hz.sxryk.cn/gtxpbfkgfk.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtvncrsvux.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtdrlnlhbu.html

PHP:  $u instanceof User
来源：http://hz.shangyingyoupin.top/gtqodwkolb.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtjiavafew.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtcfuankst.html

Java: u instanceof User
来源：http://hz.yj20258.top/gthfqfmxxy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtqrwbqjtv.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtojbczcyz.html

C#:   u is User
来源：http://hz.jinqigfzy.top/gtouxehfty.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtytgdcgpa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtkdulgacf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtitbqndhh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gtlbtomkvq.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gtwklzypwg.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtltobrwho.html

Go:   type User struct { Name string; Age int }
来源：http://hz.havefunace.top/gtlubypckg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtbmghghzn.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtozfzdyla.html

[G15] 枚举
来源：http://hz.haohaochexian.top/gtcgmusjtj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtlomgrpzr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtwotelhul.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.316326.xyz/gtgdawnvdp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtpzzuqllf.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gtaixpzmvi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtxorrjrrb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinyuanbaomall.cn/gtdlhuiyij.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtjkgpcvuk.html

[G16] 对象转数组 / 字典
来源：http://hz.vqdsnc.cn/gtnzfldooa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhaomingkeji.xyz/gtjmsqnnpu.html

PHP:  get_object_vars($obj);
来源：http://hz.birdmap.top/gtouisfcef.html

JS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtxiicvyrg.html

TS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtwpsziiwf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gthjeqbnae.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jiagoushi.top/gtfohnxktd.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtljkylzno.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtfkeivfsm.html

================================================================================
来源：http://hz.ehwqpu.com/gttxfdfpnz.html

H. 异常与错误处理
来源：http://hz.tian-w.cn/gtombhowey.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnxmvsdxr.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtnvzwyfcq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gttolnarra.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtbjqbixhs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtuwzjrpkx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gtnuvnopiy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtbldjajym.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xylfe.cn/gtzypbefxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtghvurmph.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sysykeji.top/gtzphcicwx.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtnzjvnlmz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtgunwzzmt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtwsxpgxku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtgikmzjxf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtbyhspvqo.html


<!-- 参考信息 -->