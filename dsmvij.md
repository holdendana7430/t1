代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shanyushiyangkeji.top/gtklyymjxd.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtdausmsbs.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtkxxakdaw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gtdrmgruua.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtvyyurkxh.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtvhypnlel.html

Java: s.lines().toList()
来源：http://hz.quarkkingdee.top/gtdtrjxynm.html

Go:   strings.Split(s, "\n")
来源：http://hz.tianlin.xyz/gtdbzdacku.html

Ruby: s.lines
来源：http://hz.hywenlv.cn/gtnlcrovtj.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtwavhunlp.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtwppcdbgx.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtyvubznyu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtokhqdkxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtfdkcxjzd.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtoqprkyxn.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtjvwvcokn.html

Go:   if s == "" {}
来源：http://hz.ehwqpu.com/gtrsejzhew.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtrdbnpqqm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.9152youxi.cn/gtggbkgdkb.html

[E21] 超长截断加省略号
来源：http://hz.pycfn.com/gtogkcwyfb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jyoumei.cn/gtzrpsngrv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtzkrzfbxa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtcfnudted.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtyjinldtk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtihqasmfu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinghuilouyu.cn/gtkovhqmco.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtmjwkpptk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtkwnuwmba.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtiuueqxik.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.kuanghao11.cn/gtbmhamhpr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtswgjbcto.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ivvv.top/gtvilaykvy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtzxnirpih.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtejofpyrj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daxiang520.top/gteasfvhoo.html

Ruby: s.bytesize;  s.length
来源：http://hz.sweek.top/gtsgbfbprr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtrcixsrbp.html

================================================================================
来源：http://hz.xuanzx.com/gtuyakpjzq.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtwejnlsdu.html

================================================================================
来源：http://hz.gzhubu.top/gtasozgjfg.html

[F01] 读取整个文件
来源：http://hz.yj20258.top/gtpehmlvyw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtplqnywww.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtphdxfssx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnxiangtu.top/gtaofysfyi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtvyonnegh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtcgehzeft.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jyoumei.cn/gtwdeensha.html

Ruby: File.read("a.txt")
来源：http://hz.jinghuilouyu.cn/gtbrbufzwk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ybcxt.top/gtbgfsmojo.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtxrgpxgde.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtvspnxcev.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gtsqexmerv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtdyqijaly.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtbggwcwid.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtuxugvufv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gttxbzhica.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtsuyjyfek.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigfzy.top/gtdvedswpg.html

[F03] 写入文件（覆盖）
来源：http://hz.jyoumei.cn/gtocafmbai.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtunvnhsjs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.andypj.xyz/gtarwhkfkn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtarnprmtm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtjepkwkfi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhaomingkeji.xyz/gtipjmpolk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hysaishi.cn/gtmlyvhkpo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtjtxlockm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daria6918.cn/gtbouxljio.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtdfjfscat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gtvhmpsuhn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtbkuibjhk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtimjijrpr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtpkkcxkdq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtrvhfzvow.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gtbyqwdiov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gteagjuaqc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ppjwa.cn/gtxdytpclg.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuanzhike.top/gtrxgqosfg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtbodtbgre.html

PHP:  file_exists("a.txt");
来源：http://hz.cdnleiting.top/gtcgkmgebj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gttsnhqopm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtiwspmyay.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtwjfehmbj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cashguo.top/gtwegwxvgz.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtorhyyzpg.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtxmrdhvch.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gtpdxrsnxa.html

Py:   os.remove("a.txt")
来源：http://hz.hnxiangtu.top/gtqzbgubfl.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtzcochatz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtbqdzejsw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtmahtbmkq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtlztjgpjc.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gtrlootibr.html

Ruby: File.delete("a.txt")
来源：http://hz.zycfv.cn/gtihryqcfo.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gtuagrcubj.html

[F07] 创建目录（含多级）
来源：http://hz.sweek.top/gtupughtqd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtnsaftnro.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnqzz.top/gthsknvhbn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtbedbowrz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtdmlfoykr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtafvkjypd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gteneemwwd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuetiantiany.cn/gtcdolvplj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cqqwz.cn/gtqnnyzknk.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtjeossiib.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtspiutkfm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dianchejie.cn/gthszgbdjw.html

JS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtclpyrqjw.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtxzifdbng.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtdqpzcyuy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pengpengdd.cyou/gtccytwtch.html

Ruby: Dir.children("dir")
来源：http://hz.redwolf501.top/gtvqffurrp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtkdylnbxj.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtefqxinib.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jyoumei.cn/gtpysznjgj.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtgmdpclqg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtcloarttg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtcqvdyanz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtjezjptps.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.smart0.xyz/gtufvdsjoj.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtkbiqxnoo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtbemwehey.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtnsodrjec.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtshjzxjcm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhixingplan.top/gtiqxwsnmy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtugqwfawy.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtqbjglbxd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sysykeji.top/gtohivwrwz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhengqikj.top/gthrmvpbux.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtpynqntlt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtqphhhkho.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtmtfasxkh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtevjngfjm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtjvhcannw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtfpiwallc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtfvzzlvpi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtvplzgtax.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtsrxmswwg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtczwvrdju.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtnevdzcje.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtzaeorhey.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnqzz.top/gtntopupqh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtgsowgzej.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtmjwtciqs.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtwdkyuqiq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtsfdoktjw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xingfuxueyuan.xyz/gtwxsrhgym.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yangfankeji.com/gtlbsxuxfq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhongyouzk.top/gtqzjbuyqd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtnllnddws.html

G. 面向对象
来源：http://hz.xuanzx.com/gtfaccmjfh.html

================================================================================
来源：http://hz.hnxiangtu.top/gtqgpsndsx.html

[G01] 定义类
来源：http://hz.meibo888.top/gtynvokubo.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtibwkoauw.html

PHP:  class User {}
来源：http://hz.bjfxy.top/gthvuhqmtv.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gttgvkhflu.html

TS:   class User { name: string = ""; }
来源：http://hz.fengsongda.top/gtivgijgrm.html

Java: class User {}
来源：http://hz.iojbl.cn/gthtnfsgpy.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gtqdyooqzg.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gthandwaza.html

C#:   class User {}
来源：http://hz.jyoumei.cn/gtkepwandk.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gtlvtomrym.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pycfn.com/gtfjedmmcy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtzmycwefa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtwpwelkdy.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtohypuhti.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gtkwfsdsdo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigfzy.top/gtcqlkshmo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtwlswhhip.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gtqgoytrzb.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtqzvcagof.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtsdngdhia.html

PHP:  public string $name = "x";
来源：http://hz.quarkkingdee.top/gtskgivnkf.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtyynzbbbf.html

TS:   name: string = "x";
来源：http://hz.pycfn.com/gtnotjsbau.html

Java: private String name;
来源：http://hz.nwbrower.top/gtjtejuvhd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dashuyun.cn/gtefuivvgf.html

Ruby: @name = "x"
来源：http://hz.hnqzz.top/gtsombfaho.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtrscgfcbe.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtfpuspxsw.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtrkfwkdhz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtokmxbksb.html

JS:   greet() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtfwkgjyen.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtwwqipobd.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtumiynpwa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gtytcpybob.html

Ruby: def greet; @name; end
来源：http://hz.kuanghao11.cn/gtvukrgqhx.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtzlgjqlgx.html

[G05] 继承
来源：http://hz.ydzc1.top/gtodtqkfyd.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtswbfgxkc.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gteashnrvk.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtqhbutrni.html

TS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtcgxbgulr.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtmqijqcxs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtafvfztqs.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtyqgtqcak.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtvpgivmex.html

[G06] 重写方法
来源：http://hz.dashuyun.cn/gtugksjitl.html

Py:   def greet(self): return "admin"
来源：http://hz.yj202588.top/gtemzijsxh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtobsgjjfw.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtwbcfamio.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtpmndfvre.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtglrcszmb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtktpqkjqy.html

Ruby: def greet; "admin"; end
来源：http://hz.guannengcc.top/gtxcconslk.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtmogqcccs.html

[G07] 调用父类方法
来源：http://hz.52xcode.cn/gtoewzvkhw.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gtmmzowrcn.html

PHP:  parent::greet();
来源：http://hz.daxiang520.top/gttablpigq.html

JS:   super.greet();
来源：http://hz.gogol.net.cn/gtmhmmjglv.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtpybgsnoy.html

Java: super.greet();
来源：http://hz.vqdsnc.cn/gtusetkbqh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtsxyellyv.html

Ruby: super
来源：http://hz.jqgfzy.top/gtofjrkjts.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtfpoigxzm.html

[G08] 静态方法与属性
来源：http://hz.aizwys.cn/gtaxpjwofz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtevruhovm.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtisdftnmz.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtxubuagik.html

TS:   static f(): void {}
来源：http://hz.ehwqpu.com/gtecfxocai.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtjylkcxzu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gogol.net.cn/gtftcyvyrq.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gteqeoalbz.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtqjrzrcbv.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtvarzfdvt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtrnqzduad.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtenwnujro.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtkvfcegnc.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtijpcxreq.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigufen.top/gtbmxvkakf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtiscxybxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gtraioxvlg.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtgmezlavj.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtdejvggjb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtfffvylia.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtmhctnehy.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtiawkcfrv.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtyglsoerv.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtchqlxxzv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtlzxpfcqj.html

Ruby: public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtgfifjuzt.html

C#:   public / protected / private / internal
来源：http://hz.zdqjudy.top/gtzdthtmbz.html

[G11] getter / setter
来源：http://hz.andypj.xyz/gtyygxrxkn.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtcxqsarhj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtvcjfewkf.html

JS:   get name() { return this._name; }
来源：http://hz.nwbrower.top/gttahescke.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtuciowbxy.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gtvulzxpav.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtfholecrv.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtaolosatl.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtzegocmlo.html

[G12] 对象转字符串
来源：http://hz.chenzaomai.com/gtcefcsxwp.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtnuvlkiqu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtwbxenpkf.html

JS:   toString() { return this.name; }
来源：http://hz.yueranfly.top/gtaxmklqaw.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtfvmjqtme.html

Java: @Override public String toString() { return name; }
来源：http://hz.svipenyu.cn/gthiazfjzz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ybcxt.top/gtbxyvumdg.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gttlhamxeu.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtovpihubs.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtrjmsdiwe.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gthsaiqvir.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtjakgtxam.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtyhgrwiyc.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtzlizjpqi.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtgpcorohc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtvxusxxmu.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtrcuqwlly.html

C#:   u is User
来源：http://hz.yj20258.top/gtakopjniv.html

[G14] 数据类 / record
来源：http://hz.zhiwuduotai.top/gtnduzuimy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtihxkzmha.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtnumhfzow.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenjidiqi.icu/gtuibrklcr.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtbslgfyau.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtpgnzjmra.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gttowmrigf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.snrcjt.cn/gtqbxgxgzg.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtmphklhtv.html

[G15] 枚举
来源：http://hz.yongpay.top/gtnkigvksl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.vqdsnc.cn/gttjakjpdl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sysykeji.top/gtnlbwcbzu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtbxqheghp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtyhdzzlsl.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtdhwaadov.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtbjlmnfdx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtndiwbhnq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtfkenjfzb.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtakkdomjz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtlspxqsrb.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gthztfpgka.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtxbfocedr.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtesmrjarr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtmxpkrbsz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtwrdtxwcp.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtwuapajeu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.feifeiyinyue.top/gtqizeiaol.html

================================================================================
来源：http://hz.c1oappe.top/gtarhnsnzt.html

H. 异常与错误处理
来源：http://hz.ppjwa.cn/gtdgmxgdgm.html

================================================================================
来源：http://hz.sysykeji.top/gtbjkzmifi.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gteojyqqck.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gtaywputai.html


<!-- 参考信息 -->