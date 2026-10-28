代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtvoooqczv.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtszbphdao.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtfvoxtfsc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtqrazwmza.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtnfyaahjs.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtgtermgef.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gtcfrutkwg.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj202588.top/gtnroaxplo.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtgysapowg.html

C#:   s.Split('\n')
来源：http://hz.gaohongyu789.top/gtywmdkhsj.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtyuzitysy.html

Py:   if not s:
来源：http://hz.gogol.net.cn/gttflmchzi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.bjfxy.top/gtmyjcwmjd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gzhubu.top/gttbzhvimt.html

TS:   if (s === "") {}
来源：http://hz.mhx1999.top/gtjzwntofv.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtbvnsgniq.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtbtrgitpo.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtwxghbkkq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hysaishi.cn/gtwifpeuax.html

[E21] 超长截断加省略号
来源：http://hz.fzhhl.top/gtrpjrnpob.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.meibo888.top/gtuvteuujv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtnedhjwmb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gttplafjuh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtwhbdfilg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtlvrcfyua.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gtmrlwueuz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.52xcode.cn/gtuhfprira.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtsbnjbybb.html

[E22] 字节长度与字符长度
来源：http://hz.shangyingyoupin.top/gtnebikgnt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hysaishi.cn/gtbglnrqxu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtkrkjdawj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtdofzgicm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtketqokew.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cqqwz.cn/gtcsmrbxsr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtadcwtnly.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuxming.cn/gtosesbjnk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtcazkzzem.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdpfwjmqk.html

F. 文件与目录
来源：http://hz.pengpengdd.cyou/gtcpjycmji.html

================================================================================
来源：http://hz.guowangkeji.top/gtvtgbbdbq.html

[F01] 读取整个文件
来源：http://hz.tian-w.cn/gtyfrbqjfi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtvddrnvmg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtsmycanlj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.haohaochexian.top/gtpvyomuzb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtfmyxvsjv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtufgezfdk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtfwfsbgai.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtqsymwjzy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ppjwa.cn/gtsqpjiuge.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gtclncedwx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtrvsdmkiu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigfzy.top/gtujizjfbs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtylycsavp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtwgzzyloi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gttcnefhpv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhoulong.xyz/gtueirfyme.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zdqjudy.top/gtlhbohatn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtoodljnvg.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtsmykjjjh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtvqffhqya.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtwdupzhih.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gtnyuksaxl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtdaeogrho.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.mhx1999.top/gtzyovfjuj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtkrcvwzjg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tanke756.top/gtitglkaxs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gttyuegkfz.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtxbkvujym.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.0kj1m.cn/gthkuqpgdr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.9152youxi.cn/gtoomxbozk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtzbjnylih.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtvkiimfkc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtaaggltag.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gteysppuxi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtgbvktjbv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hywenlv.cn/gtkzfridkb.html

[F05] 判断文件或目录是否存在
来源：http://hz.quarkkingdee.top/gtortmskvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgufenzy.top/gtxgkvyjyi.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtsibzdcui.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gthhbroqcp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtxnxuetqg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtbqdxezjn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhongyouzk.top/gtfenavytw.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtmtkejzil.html

C#:   File.Exists("a.txt")
来源：http://hz.birdmap.top/gtrlawanqv.html

[F06] 删除文件
来源：http://hz.hammf.cn/gtmempmgxu.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gtdqnttgum.html

PHP:  unlink("a.txt");
来源：http://hz.chenjidiqi.icu/gtqkompwuv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtrfvkfogl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtbxkabhci.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtbirwrqou.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtmoirdyll.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtfqdaqnny.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gtumeqsuli.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtceknnrbd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtsinziuzu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenzaomai.com/gtaecgymdz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtpxtiomrc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtvxovhiyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gtptexpfod.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gogol.net.cn/gtcbxwieqk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydjk.org.cn/gtukmjiiow.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.birdmap.top/gtkdwlrmlh.html

[F08] 遍历目录
来源：http://hz.nanxuanxn.top/gtutyenpgd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gtyxuedwpr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hywenlv.cn/gtmbfanafj.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtzkqkowrt.html

TS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtfayyfkem.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtcxhiwjwq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinghuilouyu.cn/gtagxqfzfu.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gteqaofyoq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtfcuutnzb.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtggwozojg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj202588.top/gtyjlcyzvi.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtagzzgndp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtkmkkpgsi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtdnvytykn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtzivisvnm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtecempcun.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtacwkepub.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtdyattobs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtvxuxkjmv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtnwisnzjb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.9152youxi.cn/gtcttgnqlh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtzirijjci.html

TS:   path.extname("a.txt")
来源：http://hz.hammf.cn/gtllajxzrz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtwugxudtu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtjqbxhoct.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtwbxhrzce.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxjhlzcex.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtdbirvbim.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtianexpgq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.redwolf501.top/gtdboacain.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtzysxbmyd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gthicrzuro.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtghumuqww.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hywenlv.cn/gtbcxkqixx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtnndmcqhd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jyoumei.cn/gttojdlbhw.html

[F12] CSV 读写
来源：http://hz.jqgfzy.top/gtrnkucojt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydzc1.top/gtuqydnnfp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gtystcymna.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtfbxbhlro.html

TS:   // 同上
来源：http://hz.ivvv.top/gtladcossc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtirqqjdzo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtgidokyow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhongyouzk.top/gttyhaoway.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.havefunace.top/gtdoeheoww.html

================================================================================
来源：http://hz.cucudq.cn/gtzdhlznaf.html

G. 面向对象
来源：http://hz.c1oappe.top/gtzwjyfimq.html

================================================================================
来源：http://hz.ehwqpu.com/gtgferhdxt.html

[G01] 定义类
来源：http://hz.yongpay.top/gtzcatruqm.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gtdorzzrlj.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtiizecekf.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtozcdxsen.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gthoayqnew.html

Java: class User {}
来源：http://hz.sysykeji.top/gtcmomdoqb.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtjnwxvsch.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtzenrmzdg.html

C#:   class User {}
来源：http://hz.redwolf501.top/gtijrrmcmx.html

[G02] 构造函数
来源：http://hz.cqqwz.cn/gtptrrzdvo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtusvoqrkq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtmcftdizs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtdrgqrxwe.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtqabcswbf.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtshiqcyqc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtopzaewda.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinghuilouyu.cn/gtdyfmnbjh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenjidiqi.icu/gtkuwqclhh.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtjgdgonaw.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtjpisyziw.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtwdkyrjgl.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtuewgkwsd.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtldmpkswb.html

Java: private String name;
来源：http://hz.snrcjt.cn/gtrvdgotwd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtdvqndxhr.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtqethcrtf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gtnjvacgci.html

[G04] 定义方法
来源：http://hz.jianghu66.top/gthvksfwxx.html

Py:   def greet(self): return self.name
来源：http://hz.meibo888.top/gtazrhwmtl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtytvwvvnr.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtjtezfdje.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtimfqkmdz.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtqomnvndj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtwruqpbre.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtykijaklv.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtykwymqlv.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtdqjmqhhu.html

Py:   class Admin(User): pass
来源：http://hz.pycfn.com/gtmfxlgvlk.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtimfeibgl.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gttdrszocf.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtnfvoybnp.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtijlrlgkh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgufenzy.top/gtycjdzond.html

Ruby: class Admin < User; end
来源：http://hz.haohaochexian.top/gtokhuabpz.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtfxkzzhty.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtyxysmrhb.html

Py:   def greet(self): return "admin"
来源：http://hz.ybcxt.top/gtpuqpjnxr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtugmhbdxh.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtjpehhjpz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtjxmohnis.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtarjkewgd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtreologsq.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtbtbfiwds.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gthocesitw.html

[G07] 调用父类方法
来源：http://hz.mhx1999.top/gtuldzhqqk.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtaxyrjost.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtgilaewcg.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtkjmgqwjx.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtpeajfpbu.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtwfejonrs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gttloyqoaz.html

Ruby: super
来源：http://hz.jyoumei.cn/gtftdebsmx.html

C#:   base.Greet();
来源：http://hz.iojbl.cn/gtfldvfbmf.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtnzvvuogy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtobjgenfv.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gthdwcwbvu.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtmmcwrzaq.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gtpzitdsul.html

Java: static void f() {}
来源：http://hz.xuetiantiany.cn/gtewapmgcp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.svipenyu.cn/gtqvtkjexe.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtiavzidma.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtorlbmsvl.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gthyuxsdhi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gthhyjltpx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtduuplcjv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhoulong.xyz/gturgexwmx.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtjpbnuqqa.html

Java: interface Shape { double area(); }
来源：http://hz.hysaishi.cn/gtrlpxbtfz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtfpwrskvy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuanzx.com/gtdpssdsal.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gthhhblugc.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtndtpjmpx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtcdijegfg.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtaqdogweo.html

JS:   #private 字段；其余公开
来源：http://hz.yueranfly.top/gthboszvuc.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtgajdzuur.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtowkvxgbr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtgufgpdwb.html

Ruby: public / protected / private
来源：http://hz.zhoulong.xyz/gtwpigplfu.html

C#:   public / protected / private / internal
来源：http://hz.yuxming.cn/gtddxgqdsb.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtkdcduttt.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gthrfwtnih.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtzbxmmyib.html

JS:   get name() { return this._name; }
来源：http://hz.cucudq.cn/gttdteqkxk.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gttyxwlkjs.html

Java: public String getName() { return name; }
来源：http://hz.ydzc1.top/gtvqcypayo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gtpfrfkqvt.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtfpbqcohv.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtrpdeoaws.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gthiqlinzs.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtbqssqudv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtmzggbxav.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtjllusqlp.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gttrggqscc.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtimmyjrcv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtjtiryfcv.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtwpbmlcrn.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gttjmptnhd.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtfhaasvwr.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gthtbugkry.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtgguzqgbv.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtxkdngilu.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gttnyedezl.html

Java: u instanceof User
来源：http://hz.jinqigfzy.top/gtmyadczmk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuanzhike.top/gtkqrlxzls.html

Ruby: u.is_a?(User)
来源：http://hz.ivvv.top/gtbjnknbak.html

C#:   u is User
来源：http://hz.yongpay.top/gtgubnxqvw.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtqjonfhpo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtgjazvvno.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtezfseqmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtpxivwvzp.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtxvpovkxr.html

Java: record User(String name, int age) {}
来源：http://hz.tian-w.cn/gtyzdtptog.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xinyue.icu/gtnfimdhjf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj202588.top/gtgcpoztob.html

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gtcmtxjzmv.html

[G15] 枚举
来源：http://hz.shuidangran.top/gthxtgczle.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtjiqokcys.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxinkj.top/gtyngqpwsz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gtzudfrxto.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gthoaqpucq.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtkheofdnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtjfzpwvpr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtcdpcallr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtiznotxar.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtsoompubq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtlpimaupr.html

PHP:  get_object_vars($obj);
来源：http://hz.pycfn.com/gthttrwfmc.html

JS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtzvfemegu.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtdxyexldi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtvrgbxolq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtwvxkhzgb.html

Ruby: obj.instance_variables
来源：http://hz.pycfn.com/gttmvcikqn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtthlpdcbc.html

================================================================================
来源：http://hz.ybcxt.top/gtynjctjim.html

H. 异常与错误处理
来源：http://hz.hysaishi.cn/gtjqsgcmjf.html

================================================================================
来源：http://hz.chenzaomai.com/gtiftgnkcv.html

[H01] try / catch 基础
来源：http://hz.52xcode.cn/gtzusuiubr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgfzy.top/gtozdepbqv.html


<!-- 参考信息 -->