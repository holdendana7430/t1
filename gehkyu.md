代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtpwkpeusz.html

[E19] 多行文本按行拆分
来源：http://hz.hnqzz.top/gtiwyzdall.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gtwiotktdg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhengqikj.top/gtcwblyebf.html

JS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gthewphyio.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtaiizfved.html

Java: s.lines().toList()
来源：http://hz.chenjidiqi.icu/gtpetdhygs.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydzc1.top/gtaergpekx.html

Ruby: s.lines
来源：http://hz.zycfv.cn/gtewrliqdn.html

C#:   s.Split('\n')
来源：http://hz.52xcode.cn/gtkghmjeak.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gtqapgnxkg.html

Py:   if not s:
来源：http://hz.zhengqikj.top/gtluqwbohy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258.top/gtpwlberiq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yongpay.top/gtwapthxkc.html

TS:   if (s === "") {}
来源：http://hz.ydzc1.top/gtfbyhzvdu.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtmcvybwmo.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtbtqdftmt.html

Ruby: if s.empty?
来源：http://hz.yonumen.top/gtktbasvax.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtuqsxeide.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtblfmyxwt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinqigfzy.top/gtetmzikhu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tianlin.xyz/gtulqqohva.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtusfbxegp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gterkozssb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gttidmysxb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtofocxuzb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtpvnxpvdc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtdnebmmeq.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtanfjuchk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gteemcukmy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtcsoogfby.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtuctndvuo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtbkeiylpq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gtbeijoitn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtwrihlzwo.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtwrlikrlv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.snrcjt.cn/gteuwojeki.html

================================================================================
来源：http://hz.c1oappe.top/gtlqlmltqw.html

F. 文件与目录
来源：http://hz.xuetiantiany.cn/gtrlseilsb.html

================================================================================
来源：http://hz.tanke756.top/gtqdpgfria.html

[F01] 读取整个文件
来源：http://hz.cashguo.top/gtacgkivsv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtckcfbehf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gtrezstxuh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtfonzocrn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigufen.top/gtwhoxieqz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtrmjvvkbw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtlegpnjlf.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtfahxwmbe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fengsongda.top/gtmjrhwvru.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtjdrtqika.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuetiantiany.cn/gtieqaprgi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pycfn.com/gtqsgqqwpu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtwbettaxg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtvzbjuutz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtldxlkyms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aizwys.cn/gtgajtjxap.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtcnisuisx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sufxvd.cn/gtffcvtgvl.html

[F03] 写入文件（覆盖）
来源：http://hz.zhengqikj.top/gttkekzvhd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gthnvjepbl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xinyue.icu/gtvovvksuw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtjsfuuemj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtivlppknp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtjcvdrtuc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.quarkkingdee.top/gtlpsnxmqp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yangfankeji.com/gtuttbvgoj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtwkrkrwdl.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtceboamdr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhiwuduotai.top/gtvvrxsvmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtzhpjxasr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtbylqmozu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtojmwhpix.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtbvdgirvz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gtadpmmpct.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtucgiyojt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.redwolf501.top/gtvtgyvqio.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtgfhzrllk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtdwrhegwh.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtnlblrnqe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmlgwjrqs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtslflqrpe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtebhtfyja.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cdnleiting.top/gtztjkepyx.html

Ruby: File.exist?("a.txt")
来源：http://hz.daria6918.cn/gtluafrohb.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtclnsuhht.html

[F06] 删除文件
来源：http://hz.feifeiyinyue.top/gtqnyfyfxu.html

Py:   os.remove("a.txt")
来源：http://hz.jlsjyb.cn/gtvhibzunr.html

PHP:  unlink("a.txt");
来源：http://hz.chenjidiqi.icu/gtltwacwfz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtiwduphzj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtpkcrlget.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtpasbewuk.html

Go:   os.Remove("a.txt")
来源：http://hz.cqqwz.cn/gtjucfvvla.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtlbkyrxbd.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtkdqpueuu.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtgzqpirei.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtyysyzspd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtuntagnhz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtxezrvukg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtgmgisxjp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hammf.cn/gtgmmanntt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yangfankeji.com/gtnhcauecw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtsvmpzjdr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtnvwykjbu.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gtofzojrjs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gturdjtvqw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cashguo.top/gtlrrholkb.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtxcrzssjy.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtzptumlsb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtybklrwmu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gthhgjajiv.html

Ruby: Dir.children("dir")
来源：http://hz.wangdashe.top/gtjrxxziwt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cashguo.top/gtsuzwudfn.html

[F09] 获取文件大小
来源：http://hz.chenjidiqi.icu/gtxaoreiwj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jyoumei.cn/gtqaytmsdn.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtmqdfsbdk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtudgqdhmr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtwpbklfdy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtvljcztfh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gtscodfzuy.html

Ruby: File.size("a.txt")
来源：http://hz.aizwys.cn/gtnljmhvou.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cheryme.top/gtcsnecdgw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtxcjrabjx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gthcncjfzn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pycfn.com/gtuiezovny.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtarajaczj.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gttdbpsddo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtajvxmjoy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtzypylzig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtrfugblds.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtdobcwgjw.html

[F11] 复制与移动文件
来源：http://hz.gzhubu.top/gtkjcbbigh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtuvotogwo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtcecathin.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtwluaomcn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtznywomst.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenlongwang.top/gtpbwdkpuk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gteiayliid.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtacbjfbul.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtkknodqca.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtbwmkvdtf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fzhhl.top/gtjurzbkxk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtsypqgxee.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtkkowwiwa.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtjdsrhoar.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtygtsnnya.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtisopbvqc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtevcfenfv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jyoumei.cn/gtnpubnhdn.html

================================================================================
来源：http://hz.ivvv.top/gtatgdcpco.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtpehahgwq.html

================================================================================
来源：http://hz.cqqwz.cn/gtoqnrwkyv.html

[G01] 定义类
来源：http://hz.yuxming.cn/gtfqozxozs.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtnkcpeitt.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtiqoxkvfd.html

JS:   class User {}
来源：http://hz.hongshengwenyu.top/gtpcbveqzg.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtiamehayd.html

Java: class User {}
来源：http://hz.mhx1999.top/gtxtlhacif.html

Go:   type User struct { Name string }
来源：http://hz.zhiwuduotai.top/gtgispmkcz.html

Ruby: class User; end
来源：http://hz.daxiang520.top/gtqoqdguhj.html

C#:   class User {}
来源：http://hz.aibaodan.cn/gtipzrsgsn.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtetupwsnv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gtkmodtsvw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtvgktogbh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtxxajyfqi.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtstbqwmla.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtmgnitgym.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jiagoushi.top/gteqxeeygy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtueypynbx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtbyducngy.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtkulgqwxt.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtjuaziarj.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtarlxrbme.html

JS:   this.name = "x";
来源：http://hz.hfpthk.cn/gthbkytbon.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtlwoeqzkk.html

Java: private String name;
来源：http://hz.ydzc1.top/gtkyhclrju.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtybtgpguj.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtqjjylegc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtfbkirrpk.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtzvxvrikv.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtuulvkapm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gthybkdywh.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtdigipqgy.html

TS:   greet(): string { return this.name; }
来源：http://hz.mhx1999.top/gtxqvzjwqt.html

Java: String greet() { return name; }
来源：http://hz.sysykeji.top/gtvigmdvet.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtjidpworr.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gtzairvwaz.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtmhddxrok.html

[G05] 继承
来源：http://hz.jinyuanbaomall.cn/gtlbsxeaon.html

Py:   class Admin(User): pass
来源：http://hz.ehwqpu.com/gtcghgsvgx.html

PHP:  class Admin extends User {}
来源：http://hz.shzxlz.cn/gtcqcfhmkw.html

JS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtzyakpqid.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtinoozfbw.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtbdigdeeo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtayflbqrm.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtotneriuh.html

C#:   class Admin : User {}
来源：http://hz.aizwys.cn/gtptkqtqgi.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtabklcgir.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gttdxodfaf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtivxhkhsi.html

JS:   greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtjsyfgvej.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtmvtaqnhp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtymicvhcj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtfbmbcfkh.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtvydsrvdx.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtrhlrnwjw.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtmdpnugae.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gtyzmbfkce.html

PHP:  parent::greet();
来源：http://hz.xuetiantiany.cn/gtpiasjtiu.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtgunvjvwu.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtuorvvsrf.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtmyuydzmy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtleorbdct.html

Ruby: super
来源：http://hz.hongshengwenyu.top/gtdlwaozgl.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gteahjnymj.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtxiuvomct.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuetiantiany.cn/gtvxboeaia.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gtzpiserci.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtnikjwoaw.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtmgyowvmq.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtqsjajonb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtfnsjrzfi.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtxbspwpnd.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtuhnsnubb.html

[G09] 接口 / 抽象类
来源：http://hz.hfpthk.cn/gttzindcfq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gthdikkzal.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtzatwelxy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtqierrbpt.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gtfjvlnrvp.html

Java: interface Shape { double area(); }
来源：http://hz.jlsjyb.cn/gtdcsmdcbl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgfzy.top/gtmdfqeuvt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtbbejolis.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtgxraekcf.html

[G10] 访问控制
来源：http://hz.hongshengwenyu.top/gtzstickia.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtxvtzlpyv.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtfwvpfgkr.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtshyzthyu.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtpdgorvma.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtnlqvqpks.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtgaejsvbe.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtzywmioon.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtymaujagy.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtksaqjvxg.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangtech.top/gtsvmdvlqh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtowgacunx.html

JS:   get name() { return this._name; }
来源：http://hz.ivvv.top/gtrkavszwh.html

TS:   get name(): string { return this._name; }
来源：http://hz.andypj.xyz/gtbmzzrrwo.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtkrmuxznz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hywenlv.cn/gtsegfvzxd.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtqofdfvuq.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gthirekljq.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtzyzdjrni.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtvtljbcjq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtlgyruzde.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtroomqspk.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gtosaxhmih.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtjqlljzsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtvqzplmwa.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtlhujbhfb.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtytgywenk.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtlunupigy.html

Py:   isinstance(u, User)
来源：http://hz.hnxiangtu.top/gtmtzwxyma.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtoylghzni.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gteilzaoyh.html

TS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtpcgqrlsy.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtspahsvac.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtndjbwnlt.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gttfiafejc.html

C#:   u is User
来源：http://hz.yonumen.top/gthccoqqcc.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtosyesbll.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtzujcqiqp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtxmbjochg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtzgxjlesh.html

TS:   type User = { name: string; age: number };
来源：http://hz.bjfxy.top/gtrxftofyz.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtewchmlwk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtlvxtbyaw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.iojbl.cn/gtaeqtfgcs.html

C#:   record User(string Name, int Age);
来源：http://hz.bjfxy.top/gtdlorovzv.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtswnbhqcr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtinireexm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtaewdtjli.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gtzerwyybx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtsvcmihwr.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gtmnsruyee.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtynlyyobm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtuhsxntgu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gtdhymgnzw.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtpsagmlcj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cucudq.cn/gtygvmuoma.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtpyaqfwje.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtpbsqszpd.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtjsrlruua.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigufen.top/gtjhbpeygw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtlmoyctsj.html

Ruby: obj.instance_variables
来源：http://hz.wangshuangyany.cn/gtkcwmyngs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtkopyetiq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyguxsujw.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtoodkfntq.html

================================================================================
来源：http://hz.birdmap.top/gtlsvlxppo.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtvqumzsmz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.bjfxy.top/gtgupujhrq.html


<!-- 参考信息 -->