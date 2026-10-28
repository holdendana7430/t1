代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gteuvdvrmx.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtrhnzlnco.html

Java: s.lines().toList()
来源：http://hz.jqgufenzy.top/gtmyvfcdte.html

Go:   strings.Split(s, "\n")
来源：http://hz.aibaodan.cn/gtwkwulyqk.html

Ruby: s.lines
来源：http://hz.wangshuangyany.cn/gtosdyisvv.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gthxevqpbr.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtyllkxfzj.html

Py:   if not s:
来源：http://hz.yj20258888.top/gtbvcnvxpl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gttifpuenu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtfyqfmyhx.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtjwhcfpru.html

Java: if (s.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtzxfwodjq.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gttfdxbmfc.html

Ruby: if s.empty?
来源：http://hz.ydzc1.top/gtwyyfzlhg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtwpzpephi.html

[E21] 超长截断加省略号
来源：http://hz.sxryk.cn/gtqdtpuhuu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtflxmhawz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtmagzlhhl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtrakjhphx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtzuvltcjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtjsbaepax.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtntocweos.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigufen.top/gthvvyzmmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtdwbvbcvm.html

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtsrbymsgj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxuanxn.top/gtccowriis.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtrmmynakz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtwyovcyks.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtczuqwzlp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.mhx1999.top/gtvkpsdyqt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gtoithlhtf.html

Ruby: s.bytesize;  s.length
来源：http://hz.gogol.net.cn/gtjtdnjtqk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtnqyhbwzz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtilxxayhd.html

F. 文件与目录
来源：http://hz.daxiang520.top/gtilodvckn.html

================================================================================
来源：http://hz.pycfn.com/gtqgkwtctb.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtxiowommy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shanyushiyangtech.top/gtutzphway.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtwlitprsq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gttaxqajek.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jyoumei.cn/gtqblnxczy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtbgcgrdny.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gttfcpckgz.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtcaozgrdb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydjk.org.cn/gtbxvnporr.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtzsufzfcb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.redwolf501.top/gtrtxoebje.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gtzbdfjbbt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtcxqgsysi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtijlzkjlv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtauaqdwco.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtmysfuldy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtqanueccw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtnxjnvtxs.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gtqrzmvxdl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtysdvjmiw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.c1oappe.top/gtadqgzpsm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtodyejtmv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtqwhougzi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xziqi.cn/gtzfqoxgwu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gtspozktkc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtwplwwgou.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtotggsbsd.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtzspksibx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtqirdtoyt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ybcxt.top/gtmafboceh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtvedwxqyc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtknlsrgyl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtozikbppx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtredyawav.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtlbxtjrvv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtnkldosrh.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtzgejctna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtxocwcsye.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtkokugntb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtdeujpbah.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtauhxutqd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtmwcpxykl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtskoepjon.html

Ruby: File.exist?("a.txt")
来源：http://hz.zdqjudy.top/gtavmhlkmq.html

C#:   File.Exists("a.txt")
来源：http://hz.zycfv.cn/gtsxvvapkd.html

[F06] 删除文件
来源：http://hz.sufxvd.cn/gthafxfplv.html

Py:   os.remove("a.txt")
来源：http://hz.daxiang520.top/gthvelyxwq.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtmjsjldkm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtnotriekb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtzohcjnyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtfayddxsk.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxyfdzyed.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtpemujayw.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtddmeqdtc.html

[F07] 创建目录（含多级）
来源：http://hz.shuidangran.top/gtsynuultc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtswrfaltu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtxwvzxyhr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtlbxgplrm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtwumfeuff.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtzcapbhbs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtouirarjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gttarowtew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtbvaltjrt.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gturewedin.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtpivkxmym.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtpayopicc.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtjecfcnka.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtwortcezh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtidselxok.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhijiandao.cn/gteftltxfw.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtwgnsftqr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gtmlvtjzpi.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtjxatlcle.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtsayivups.html

PHP:  filesize("a.txt");
来源：http://hz.daxiang520.top/gtsjwezqxn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtprjzfozo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtcyuiwqak.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtpknclchm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtkddshphs.html

Ruby: File.size("a.txt")
来源：http://hz.cucudq.cn/gtinnwehax.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtmwckhdul.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtxpfsaasi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gthrzjecst.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.bjfxy.top/gtuslbpqpa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtrylfsyms.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtnrujcudt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtixjqyqbv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtocsnnyrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtinhfddvl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtzxmkxzkj.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtlftbyiwm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtqoafyrfh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtieotgysd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtmmnwmrbi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gttjmcfhlo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtqwnjnxvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gticnmscbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtkekkxtuc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtxwzubbir.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gtkfrqhyzv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258888.top/gteqeiqahj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgufenzy.top/gteafrmqfq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtnaqyesdh.html

TS:   // 同上
来源：http://hz.xinyue.icu/gtatzuedqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xinyue.icu/gtanmuryyd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtoprobfoc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gttcvazlbf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gtrihxvsqt.html

================================================================================
来源：http://hz.tanke756.top/gtzzzzhuhm.html

G. 面向对象
来源：http://hz.sxryk.cn/gtlcvlnawv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmqtvndhn.html

[G01] 定义类
来源：http://hz.jianghu66.top/gtozddmovf.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtxzemmcsh.html

PHP:  class User {}
来源：http://hz.ivvv.top/gtsgktqwbb.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtkkrakodr.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtcodvhplg.html

Java: class User {}
来源：http://hz.guannengcc.top/gtqssceahv.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtfmglvdgl.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtbyviztsv.html

C#:   class User {}
来源：http://hz.guannengcc.top/gtjrqnsxdp.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtgxxnigvt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtjcifpohj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuetiantiany.cn/gtxfnwnrlb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtwcbecqrm.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtmotinmqy.html

Java: User(String name) { this.name = name; }
来源：http://hz.smart0.xyz/gtfhksscnb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtktiuwbal.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.haohaochexian.top/gtdfgcrybo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yanxiufei.cn/gtsoygelxs.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtbqlhskyk.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtqjjzverm.html

PHP:  public string $name = "x";
来源：http://hz.jianghu66.top/gtfogrdsxj.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtxgwhzaqy.html

TS:   name: string = "x";
来源：http://hz.ydjk.org.cn/gtsxroymep.html

Java: private String name;
来源：http://hz.ydzc1.top/gtqhlselzj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtynksxnsh.html

Ruby: @name = "x"
来源：http://hz.jyoumei.cn/gtjneqxktg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtufeyejbu.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gthhdsltis.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtwrpvimkv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtgrgpzhzi.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gtyiapmjhl.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gthbhhaybn.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtksupoaen.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtvuhlagha.html

Ruby: def greet; @name; end
来源：http://hz.yj20258888.top/gtmloavqlr.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtjbvrjjww.html

[G05] 继承
来源：http://hz.yangfankeji.com/gtlvujafbx.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtdpowbfzv.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtcsjgfpkw.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtxgdqszjp.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtjbtvzvmt.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtubpwchwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yueranfly.top/gtoynhjvqp.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gteojlhvsn.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtysidbrnw.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtsurtqnjt.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtrbbuiqvh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtgagseekh.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtqbwexdes.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtwushadru.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtxzwmwolq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtjaeyixph.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtxgoygyzv.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj202588.top/gtsdirdznv.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtbyfuigfu.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtgygmewkm.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtpajyvclq.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtfpcdhnka.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtgeaqzaqm.html

Java: super.greet();
来源：http://hz.cheryme.top/gtmhfrihpe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtdgralpkv.html

Ruby: super
来源：http://hz.cqqwz.cn/gtasywlfbj.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtiawavlme.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtudjkseju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtkltkghmc.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtalgjdlkb.html

JS:   static f() {}
来源：http://hz.ywan-chungtsiang.top/gtizjonwnx.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtzdxzagqt.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtzpfyuvjz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hammf.cn/gtflcgdcdr.html

Ruby: def self.f; end
来源：http://hz.c1oappe.top/gtpkyzcclz.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtxvucvstx.html

[G09] 接口 / 抽象类
来源：http://hz.guowangkeji.top/gtcfhubyks.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtyoytpuxz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtxvbldmmy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gtnoybtpbu.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtmnjdocal.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtrdjymrhh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pycfn.com/gtmleyhnqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtaqowhhws.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gthgksybfz.html

[G10] 访问控制
来源：http://hz.birdmap.top/gtophvpjjl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtiwlafodm.html

PHP:  public / protected / private
来源：http://hz.feifeiyinyue.top/gtgukirtsj.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtgnaduloe.html

TS:   public / protected / private
来源：http://hz.sweek.top/gttbmkkaky.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtlmwtaitr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cqqwz.cn/gtbkrrfrho.html

Ruby: public / protected / private
来源：http://hz.ydzc1.top/gtxwfftutk.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gtvpydtkha.html

[G11] getter / setter
来源：http://hz.zhiwuduotai.top/gttdhdwvig.html

Py:   @property 与 @x.setter
来源：http://hz.c1oappe.top/gtxudzunoy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtjnotdneo.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtfwpesyff.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtusrdarsn.html

Java: public String getName() { return name; }
来源：http://hz.aizwys.cn/gtzcoqichz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gtgxhtrohk.html

Ruby: attr_accessor :name
来源：http://hz.ybcxt.top/gtbfrtyujb.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtkxdafzxo.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtpqfjqvqq.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtnwqshvuo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtrgfkekzj.html

JS:   toString() { return this.name; }
来源：http://hz.gogol.net.cn/gtckjqnfcs.html

TS:   toString(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtwircdaeu.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtjridxciz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtkgppfpmy.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gthxqmlyxe.html

C#:   public override string ToString() => Name;
来源：http://hz.xuetiantiany.cn/gtpabrafws.html

[G13] 判断对象类型
来源：http://hz.daria6918.cn/gtymhessxa.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtcgsjpzob.html

PHP:  $u instanceof User
来源：http://hz.cashguo.top/gtnuorlrta.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gttdjddivp.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtmiqitgfr.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtlnnxzosr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtkwlfzqbl.html

Ruby: u.is_a?(User)
来源：http://hz.yangfankeji.com/gtzjgpdmwy.html

C#:   u is User
来源：http://hz.wangdashe.top/gtdjgudvfl.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtifqslsby.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtfpqugnzn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtdbmigaht.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtabjlfbhe.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gttybpurgo.html

Java: record User(String name, int age) {}
来源：http://hz.vqdsnc.cn/gtdmkjialr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtkfcpzvbf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fzhhl.top/gtittcjlxs.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtkidantag.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtlasgsatd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.havefunace.top/gtdynbisng.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnxiangtu.top/gtkcbuezqm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gteysyttpx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtfebnzman.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtvzflbfek.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtycyivbvn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtkivrdxds.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gthkwscmag.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtifqesbrx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guowangkeji.top/gtgnwqaejj.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtwxkocegq.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtpxmzapoq.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtsqnfgtoz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtrwlvxxem.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtpgqawmkg.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtoupxkcls.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtafiwosql.html

================================================================================
来源：http://hz.sweek.top/gtglrtvqje.html

H. 异常与错误处理
来源：http://hz.cdnleiting.top/gtzuqrugkg.html

================================================================================
来源：http://hz.zhengqikj.top/gtmcnmwscd.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtlgensbwy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtbmxdkfal.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtikyjscja.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtcsxpjvuh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtzilfgmci.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gthuftdhvt.html


<!-- 参考信息 -->