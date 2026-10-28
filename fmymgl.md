代发 wailian999

Ruby: s.lines
来源：http://hz.mhx1999.top/gtbiraocon.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gtjqiitatw.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtoklrssyu.html

Py:   if not s:
来源：http://hz.jinqigufen.top/gtmvenqvcb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtvyzlfhlw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dianchejie.cn/gtpplxrcvn.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtzigydggo.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtnqycwfku.html

Go:   if s == "" {}
来源：http://hz.yj20258888.top/gtlgbjyfsp.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gttzrnfodq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.mhx1999.top/gtauiiemcc.html

[E21] 超长截断加省略号
来源：http://hz.yj20258888.top/gtflfhigrf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.feifeiyinyue.top/gtqvvsmoaf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pengpengdd.cyou/gtdqpxzyzx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtoqxmiywt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtqtenqwky.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtybauyxpx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.svipenyu.cn/gtmfxyxjag.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtxbjsguml.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtvuxffhap.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gtejibcmsf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.316326.xyz/gtrbscdhbo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtfdcvvifo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtyfulqwhf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtgdukbtti.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gzhubu.top/gtaxjadfwp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.vqdsnc.cn/gtwthuivvn.html

Ruby: s.bytesize;  s.length
来源：http://hz.ivvv.top/gtljwkezql.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtaugjdgjn.html

================================================================================
来源：http://hz.jqgfzy.top/gtxgrpkqfw.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtoxhowuei.html

================================================================================
来源：http://hz.yuanzhike.top/gtznkxsmzo.html

[F01] 读取整个文件
来源：http://hz.guannengcc.top/gtsnzosqum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtmofllkux.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xinyue.icu/gtheuyveym.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dianchejie.cn/gtyshpjpxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtwkiktvmi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtkkmxxovk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtfiuberak.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtrutrefsp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gthjgfdkkw.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gttejdhhru.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnqzz.top/gtkqkxhgti.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gogol.net.cn/gtkrqmlhkk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtylycuikc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtukyozseu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtidouojjx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtsuwmjupf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtjushuupz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.redwolf501.top/gthyetxtii.html

[F03] 写入文件（覆盖）
来源：http://hz.guowangkeji.top/gtvgunhrox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gteqolpjts.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gttmvgwglf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtltonvymh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtqczvsekm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tanke756.top/gtbssnreuv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydzc1.top/gtprcpwosk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtoqpfvvch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenlongwang.top/gthuzdmvkw.html

[F04] 追加写入文件
来源：http://hz.cqqwz.cn/gtbbryvril.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zycfv.cn/gtlswsksnb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtvsjuxllf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtdcfhgeaw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gttyugblkv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtxcxfhvyf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtvzofmjxq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtwcrrurcq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shuidangran.top/gtdojlxidy.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtmeyhyevy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtsuqwglif.html

PHP:  file_exists("a.txt");
来源：http://hz.shzxlz.cn/gttlbsjilb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtdcwpwnoj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtkboyaykg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtvqybshhd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtonivjnrw.html

Ruby: File.exist?("a.txt")
来源：http://hz.xylfe.cn/gtfruvckvx.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtnmnizpzs.html

[F06] 删除文件
来源：http://hz.gzhubu.top/gtfagtjfsq.html

Py:   os.remove("a.txt")
来源：http://hz.pycfn.com/gtwskrjgus.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gttjlnjgnf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtrbsenrzl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtdkvoyewv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtlhdccrrr.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtjdqlwyxt.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gthjtnabxa.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtxtlpjxfa.html

[F07] 创建目录（含多级）
来源：http://hz.gzhubu.top/gtofbgiwfh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gtbfwjfsxq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fzhhl.top/gthmuskvvn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtjhtzmyoi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtpzsmnmcm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.redwolf501.top/gthxjdxyzr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtkxxabcef.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtmuqcovlm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtxmskmmtn.html

[F08] 遍历目录
来源：http://hz.nanxinkj.top/gtjipfuckn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hysaishi.cn/gtugicbatz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtmpgoqqeg.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gteqorcejl.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtzdcbwjmv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtgfmhovgg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhengqikj.top/gtxdtkzrwm.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtwblrvwxv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tianlin.xyz/gtgrhltsud.html

[F09] 获取文件大小
来源：http://hz.dianchejie.cn/gtkddwwyvd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtojrrtlpn.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtmzwkdgal.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtyusheogx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtmgthodlx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtnessfpob.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtivhguyqu.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtfoxhxjdx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhoulong.xyz/gtpdmelatb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daxiang520.top/gtumsxxtkc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtksosimsn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhiwuduotai.top/gthaamsabe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtxembcwhk.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtxaygmtex.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtgpkzffkm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtcqgawgul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtdkikasvk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtamdhxauy.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtlxralwll.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtmgjnhnor.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtpyiugoae.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtqxgxvyjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtfqkrdrae.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtwelaceao.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gtthqfymqq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtbtutguqd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhoulong.xyz/gtedvzewcr.html

[F12] CSV 读写
来源：http://hz.hnxiangtu.top/gtiwmsqeuw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtvfkaxree.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtrwlbmofo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtwkvlkqig.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtyevgkrpf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jlsjyb.cn/gtnamdeprr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gthykbibmp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fzhhl.top/gtsxojuzge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gtcwvwrvem.html

================================================================================
来源：http://hz.sufxvd.cn/gtpyimfyyu.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtxepbgskd.html

================================================================================
来源：http://hz.aizwys.cn/gtxyjpeknt.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtkwwvuolt.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gtwzlytayp.html

PHP:  class User {}
来源：http://hz.fzhhl.top/gtyubogaej.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtpfyirxdd.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtxeshhobd.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtmgmkahxo.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gtkscvslaw.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtylixmssq.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtrrqbguwy.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gthlnvsgtl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnxiangtu.top/gtfoojmdhm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtftcmevme.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gttmnrevel.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtrrtlffqj.html

Java: User(String name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gthtcbeyck.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gtsdncbkqv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtvbueqlml.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cucudq.cn/gtbjpqrppc.html

[G03] 实例属性
来源：http://hz.bjfxy.top/gtuyzddifw.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtfljpyjhj.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtblcgkmvm.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtitfokvzs.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtvxjcuwed.html

Java: private String name;
来源：http://hz.snrcjt.cn/gttvswmmhy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gthrpqmamd.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtrdqyfpbt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.havefunace.top/gtwgexomzd.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtxybgriuk.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtkstmxpmk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtmcgkibnn.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtwnmjzvaw.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtmajzdpfh.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gttcyvtlgt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtyfbihbwa.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtewpnauxx.html

C#:   public string Greet() => Name;
来源：http://hz.sweek.top/gtbwplemls.html

[G05] 继承
来源：http://hz.nwbrower.top/gtmsqadyce.html

Py:   class Admin(User): pass
来源：http://hz.ivvv.top/gtzotlkwre.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtoljpjheo.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtjhpcyrgt.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtuflpgzxh.html

Java: class Admin extends User {}
来源：http://hz.ybcxt.top/gtrplempdz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtlhqrnrod.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtmiffqifs.html

C#:   class Admin : User {}
来源：http://hz.jqgufenzy.top/gtclyhbbtp.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtmbnrbmik.html

Py:   def greet(self): return "admin"
来源：http://hz.guannengcc.top/gtadogzkxs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtzuwqvfpr.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtpmrqwmfi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gttczrggii.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtdrjmpiyz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtybcipivk.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtznpymvwa.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtfbjrwlzf.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gttliolltx.html

Py:   super().greet()
来源：http://hz.jianghu66.top/gtcnghrsin.html

PHP:  parent::greet();
来源：http://hz.jqgfzy.top/gtwnzrrqia.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtdvimodqp.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtqpepmztu.html

Java: super.greet();
来源：http://hz.9152youxi.cn/gtbgpocwla.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cqqwz.cn/gtomipgduk.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gtnaqptpgr.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtvzpfiipc.html

[G08] 静态方法与属性
来源：http://hz.0kj1m.cn/gtozbswoyy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtmhrxctot.html

PHP:  public static function f() {}
来源：http://hz.zhengqikj.top/gtlaffqdda.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtjzjxfcap.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtnotcygbn.html

Java: static void f() {}
来源：http://hz.tianlin.xyz/gtlvyokceh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xylfe.cn/gtdfgrjrha.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtkhzqkyuy.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtmveosjlz.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtiirzyifw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtzyccqfwj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gttudhvlid.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cashguo.top/gtimpdjigm.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gtopupanfw.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtnluwnsek.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gthogoytfb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtcnjqdqcb.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gtxyororaq.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtxoiegsum.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xinyue.icu/gtahiagpgb.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gtozpfqior.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtrlpfvkfk.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtggstnfzl.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtlgdmlijy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtikceizwu.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gtmqyaywec.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtrfhuhhdu.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtarvwgcqv.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gthmztnuvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtmlcqberx.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gttzvwpsho.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtjtsjrioo.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtuyuhdlir.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtitsynotl.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtmlqqniva.html

C#:   public string Name { get; set; }
来源：http://hz.dianchejie.cn/gtvibqthkz.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtacpjaotf.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtxglxcits.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtwqdqnfld.html

JS:   toString() { return this.name; }
来源：http://hz.nanxuanxn.top/gtjinrplkb.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtkqyvmtjs.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gtrtysmwgd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtxnhhrvwb.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtuqqfudsp.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gtyrdnbpjc.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gtgxpzhvnq.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gtpypjamnm.html

PHP:  $u instanceof User
来源：http://hz.jlsjyb.cn/gtnnbroosk.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtcdrhlfii.html

TS:   u instanceof User
来源：http://hz.xylfe.cn/gtbpysvkhq.html

Java: u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtnkouwcyn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.smart0.xyz/gtqgxsjmkx.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gtshuamddg.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtygjphibk.html

[G14] 数据类 / record
来源：http://hz.kuanghao11.cn/gttjtnyeax.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtfkocnytc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtvgtgntyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtohthymwl.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtsxyucbrp.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gtaamppvan.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtllmufjpl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.snrcjt.cn/gtlsmbqeia.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtwnisrstw.html

[G15] 枚举
来源：http://hz.jianghu66.top/gtbssgfhsu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtbvbzcfof.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gtsxnugdbf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gtsptvmxbx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtqjoopljc.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtybbrnuqw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtrdstebss.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtsthxndgb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gthtocrxiz.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtsxczcdus.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtlbhupokq.html

PHP:  get_object_vars($obj);
来源：http://hz.sweek.top/gtbviycmgz.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtpjjronzq.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtbdxdqnqn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258888.top/gtdygsbggy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhaomingkeji.xyz/gtnniagujn.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtpzykvhwn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtpfcmowwf.html

================================================================================
来源：http://hz.ivvv.top/gtvcxxsqxm.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtcrxwyxey.html

================================================================================
来源：http://hz.yj202588.top/gtaehpktpo.html

[H01] try / catch 基础
来源：http://hz.smart0.xyz/gtkjbrzkbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtkujjkeoi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gtfjjeeqzx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtbjmrukyb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj202588.top/gtngnvjzis.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuxming.cn/gtxdoioxlf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtwkyjwpfn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtebkcyxxk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gtvrseicei.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtgvvpmwyb.html


<!-- 参考信息 -->