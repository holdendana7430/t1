代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtiodwgxfn.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtrrvwujxp.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtubwnuwnc.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtxqtsgvsp.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtoalslpfd.html

C#:   s.Split('\n')
来源：http://hz.yvedp.cn/gtkupsxtwz.html

[E20] 判断字符串是否为空
来源：http://hz.hongshengwenyu.top/gtavdnrbqw.html

Py:   if not s:
来源：http://hz.ppjwa.cn/gtqojfmuxw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gtkboutuzh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.svipenyu.cn/gtmjitrkdu.html

TS:   if (s === "") {}
来源：http://hz.guowangkeji.top/gtjioohgxe.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtcrfayxtc.html

Go:   if s == "" {}
来源：http://hz.chenjidiqi.icu/gtoffmpofl.html

Ruby: if s.empty?
来源：http://hz.jianghu66.top/gtsfszbsti.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtefwnqwub.html

[E21] 超长截断加省略号
来源：http://hz.jlsjyb.cn/gtqaxohgsq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gtiqxivqqv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtjvmuqncm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtcmozhads.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtfleljosk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtxtijsuid.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ivvv.top/gtgmocmgac.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtjolbgxmr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.316326.xyz/gtarkdplxf.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gtnadyfvmh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtyubhamgn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gttkvlrccf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtjwqbkjmp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtrikybsxh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtyukxcsvb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.birdmap.top/gtavcikwtd.html

Ruby: s.bytesize;  s.length
来源：http://hz.ywan-chungtsiang.top/gtfpxtcoig.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtlsyvcbim.html

================================================================================
来源：http://hz.zhengqikj.top/gtkeaatjas.html

F. 文件与目录
来源：http://hz.9152youxi.cn/gtcwczibzl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjmmrmvbz.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gtlajudxdm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtgxunwhwa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtylywoiwh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ywan-chungtsiang.top/gtnabodfnh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sysykeji.top/gtbhbepbbf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtarputyqu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dianchejie.cn/gthlzgkxaq.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gthxfymjup.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtzvhtcvat.html

[F02] 逐行读取文件
来源：http://hz.sxryk.cn/gtvjktuyzr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtmhvcvjgs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gtrxkkohvp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtozqstgvs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtmjdcucee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtldrpbsmk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xziqi.cn/gtxsaqasbd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.316326.xyz/gtfrchnrnp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gtxkfiknad.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gteeqepplg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtluyqxtek.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sysykeji.top/gtqrwschuk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtfimnposg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gttgfbvxcp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.iojbl.cn/gtcicjbrfm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtxbmnnfwq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yangfankeji.com/gtzpwwvbrt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydzc1.top/gtrjlsliwf.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtihbketlp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.haohaochexian.top/gtilxhzngw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtpowvjwxp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtygqbdytx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtrlqcopee.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.havefunace.top/gtpjyvdjds.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhoulong.xyz/gtzscobudq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtpvraeilr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtnggxcolv.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtmtuktczd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtewkeuoou.html

PHP:  file_exists("a.txt");
来源：http://hz.cucudq.cn/gtcbyujdpn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtdlrzoydy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtmyixijca.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtdheiopjg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gtruqcqpff.html

Ruby: File.exist?("a.txt")
来源：http://hz.yonumen.top/gtcklaqwiv.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtsibkrcrp.html

[F06] 删除文件
来源：http://hz.c1oappe.top/gtqxakhzdy.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigfzy.top/gtirlfslwz.html

PHP:  unlink("a.txt");
来源：http://hz.sufxvd.cn/gtoauokrmn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtftxkmvhy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gthewronfa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtnjsnpqzu.html

Go:   os.Remove("a.txt")
来源：http://hz.yj20258.top/gtfbqkwbwp.html

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gtpjwafchs.html

C#:   File.Delete("a.txt");
来源：http://hz.52xcode.cn/gtotlmxqrp.html

[F07] 创建目录（含多级）
来源：http://hz.gotoacloud.top/gtbbcpgpby.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daria6918.cn/gtgdticgaj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtwgrklrcn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtckpqcmxo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gttejkeckt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jiagoushi.top/gtxsekkfen.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gthsbhwctq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtjxowgfsr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pengpengdd.cyou/gtcbzlvzhx.html

[F08] 遍历目录
来源：http://hz.cheryme.top/gtxrkifjxq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtqmvrwyln.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.andypj.xyz/gtsvtncipj.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtyokapwsb.html

TS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtrlcqlyyd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sweek.top/gtonrzoiuu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj202588.top/gtkedwgjiw.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtksyxawyy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtymvfkwsz.html

[F09] 获取文件大小
来源：http://hz.ydjk.org.cn/gteqhobonz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtbdtkwpsv.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtieaopfbf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtzsfpviko.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtfnrjfdyn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtxqbplbuj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yvedp.cn/gtgznyobbw.html

Ruby: File.size("a.txt")
来源：http://hz.chenzaomai.com/gtbpawmiso.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtqyewcddu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daria6918.cn/gttvgayfrn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpoabfhrr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtwwlziums.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtpwsobnkx.html

TS:   path.extname("a.txt")
来源：http://hz.hywenlv.cn/gtheafffem.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenzaomai.com/gtzogqhmxp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtobaygdaa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtkftwpppf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtiesrlwqi.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtewkgynvl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtzmbbrmlb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtowczxdgs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtyfktwfpc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtdzvllurw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gttzluwsca.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigfzy.top/gtzkfmylfp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtoxawtcad.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shuidangran.top/gtvzefqzbm.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtasjkspdg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtrscsqvci.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtakiaihqq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtzjavyebg.html

TS:   // 同上
来源：http://hz.gzhubu.top/gtmussliup.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtunhaqeod.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtnyabpgew.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtxdgkdjtf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtnvzjhbuc.html

================================================================================
来源：http://hz.daria6918.cn/gtkjbrhjab.html

G. 面向对象
来源：http://hz.iojbl.cn/gtejcmhoag.html

================================================================================
来源：http://hz.redwolf501.top/gtuqhspetj.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtbnndudws.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gtomnjdpdn.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtglkuopmf.html

JS:   class User {}
来源：http://hz.yonumen.top/gthnnxplgp.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtfegbrniy.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtremoikze.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtpfmkoxyo.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtltuexrfj.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtviogzlnu.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtghoxwece.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtuqlekzjw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daria6918.cn/gtxjqnjcpc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtawslsrlm.html

TS:   constructor(public name: string) {}
来源：http://hz.iojbl.cn/gthpnyklfq.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gttzhtlqlu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gtywabkxzb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtgbxlzxfs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sysykeji.top/gtggheccyh.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtpjnvfqxk.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtcvrxlnyy.html

PHP:  public string $name = "x";
来源：http://hz.daria6918.cn/gtuzvurzvx.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtitwehgme.html

TS:   name: string = "x";
来源：http://hz.xuetiantiany.cn/gtfpgljsbu.html

Java: private String name;
来源：http://hz.sweek.top/gtarnpbwzl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtngasyvqg.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtqifuwzgj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gttvuhakfn.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtvhxmyryv.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtwxkwfblp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtuyrdvwub.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtnpuiitdz.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtotjsflyu.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtfbgrtnxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zycfv.cn/gtnlfktonk.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtpzsvuydn.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gtdxwufibw.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtijdnujbw.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtrgiomlck.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gttkrmfixx.html

JS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gttxymhgge.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtjlhltvgf.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gttbrzntdg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtlrsekour.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gtklwbofzz.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtaitgjzbo.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gttjqaqtwf.html

Py:   def greet(self): return "admin"
来源：http://hz.dianchejie.cn/gttrizhsiq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtmykisobs.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtxhzxsykv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtfnkcfvji.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtcdlsjasq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gttcbtksbr.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtcifdbula.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtzrspseos.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtcusqyxdf.html

Py:   super().greet()
来源：http://hz.jiagoushi.top/gtiuqtbdoy.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtyrvhbqtv.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtdyweglvf.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtzoafnphg.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtnyxffqeo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtkifeyzah.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gtowagcepx.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtxwbxvveg.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtfuhagsco.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gtxtzrjofp.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtubrcpgon.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtashyxzxv.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtfthquavf.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtyxjkpfne.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtmeismnsb.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gttflnkjrn.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtemhampju.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigufen.top/gtstuesvis.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ybcxt.top/gtqiqohiag.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxinkj.top/gtgauwiitm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhijiandao.cn/gtqpxpppas.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhengqikj.top/gtmivhdcdm.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtyhlwffli.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gttsxsrfnq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtucghrkgl.html

C#:   interface IShape { double Area(); }
来源：http://hz.bjfxy.top/gtcfurficm.html

[G10] 访问控制
来源：http://hz.yj20258.top/gtuvjbepjf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ybcxt.top/gtzkwsewta.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtmxoqwwyu.html

JS:   #private 字段；其余公开
来源：http://hz.jlsjyb.cn/gtadoccjgv.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtzyaeiley.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigfzy.top/gtrssdlqra.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sufxvd.cn/gtcbscuqua.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtwhzemprk.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gtnafxtgfr.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtvnsnqmnz.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtxegbtnyk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtrnfboelk.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtfajxthua.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtystwslzs.html

Java: public String getName() { return name; }
来源：http://hz.redwolf501.top/gtyxoexjkx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shzxlz.cn/gtsfbrtunk.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtvuyxennw.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtueriplry.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gtlmeypajg.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtjcsmbukp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtrojvrsbv.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtqhbwxbpv.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gttgxmuylz.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtijpmspec.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtvdbohmrc.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtpxtcaveu.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gtqcoicjtz.html

[G13] 判断对象类型
来源：http://hz.zhaomingkeji.xyz/gtuidfgtil.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtqptftmln.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtmodddqtj.html

JS:   u instanceof User
来源：http://hz.nwbrower.top/gtymsjtbvy.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtecgojtyj.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtqfyobxkp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gteruhfiyd.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtsklydsrs.html

C#:   u is User
来源：http://hz.wangdashe.top/gtewdyddgy.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtpfkafhrp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cashguo.top/gtljmcwdyk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtejbjtlyc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guannengcc.top/gtutffonzh.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gttqwaxqrx.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtyfisjbwy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtkchajsde.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtlvozvnyp.html

C#:   record User(string Name, int Age);
来源：http://hz.yvedp.cn/gtfrmvhfnv.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gthzvinfhu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtjhyghklz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtvkpbcuss.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.haohaochexian.top/gtmjsdoorb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtosognbjb.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtugnicklf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtfjnpvkzl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtyioipgxy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtamojsjeo.html

[G16] 对象转数组 / 字典
来源：http://hz.yonumen.top/gtgakvdujr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtalitqqzv.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtaudjajig.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtmbngzuut.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gthfhdezal.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtbsqwjtnk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtqippvtzv.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtvsnfgska.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtskjjwobs.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwfdkrfbx.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtbytvmztj.html

================================================================================
来源：http://hz.gzhubu.top/gtpsmmlfsj.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtzpeedlzz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ybcxt.top/gtvnuzxcca.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gtibjjpcae.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtbvrlvnvz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtsvxxnudv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gtgnkknkzc.html


<!-- 参考信息 -->