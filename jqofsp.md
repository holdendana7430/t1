代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yueranfly.top/gtoubuusuo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gttfwvntrp.html

TS:   if (s === "") {}
来源：http://hz.hnqzz.top/gtyevjorzn.html

Java: if (s.isEmpty()) {}
来源：http://hz.sweek.top/gtusfqxsra.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtbwkvncna.html

Ruby: if s.empty?
来源：http://hz.zhaomingkeji.xyz/gtgyrkjjdq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigfzy.top/gtalzzizhi.html

[E21] 超长截断加省略号
来源：http://hz.ywan-chungtsiang.top/gtftpgzjwl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.daxiang520.top/gtzppsmpuk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtqiqkieyq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtvjgcrcgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtyboqqrjt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtgwzjsbmv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtqbkxtuuo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.52xcode.cn/gtgfhwulae.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtotukfoql.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gttdkixrrs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtermyaxqt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtkggcnczi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtkpmahjdb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtmohjmwsn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtkehbobtn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.9152youxi.cn/gteetocxea.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gteevkgdiy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.havefunace.top/gtuhrutrul.html

================================================================================
来源：http://hz.zdqjudy.top/gtpytxrknb.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtjgtodkym.html

================================================================================
来源：http://hz.shzxlz.cn/gtzifpvwmj.html

[F01] 读取整个文件
来源：http://hz.pengpengdd.cyou/gttxypwjaq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtdgvbgguc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gtfcqqlgqy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhongyouzk.top/gtfpgovsiw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgfzy.top/gtfnbdefzl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtsggymjdz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtpckseudd.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtuocjndsp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtsijgkgpa.html

[F02] 逐行读取文件
来源：http://hz.yuanzhike.top/gtlrtniaeq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangshuangyany.cn/gtafnulbwd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhaomingkeji.xyz/gtuhpifuqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.kuanghao11.cn/gthnxvemxm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtlicbfjcb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtqsklzroc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtdvfuogjq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gtsrvjeeki.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gtkvzckdzi.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtwkjhximu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtjklryxyu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtjtfhxnqn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtbdlsoxpx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtufdrlwsz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtcqbjxqaf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sweek.top/gtgkhmzdif.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.52xcode.cn/gttdrjldcf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.havefunace.top/gtdrlbjden.html

[F04] 追加写入文件
来源：http://hz.iojbl.cn/gtpdmskyzg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gtwoxieraw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ywan-chungtsiang.top/gtbjiwqecc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtqnjmabzy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtmvxnvkpv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtkjmrgkwv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gthrgtspzw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.andypj.xyz/gtpetmfjso.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shzxlz.cn/gtbdsunrod.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtpipyvvoq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtwhvkznca.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtzxxulqbd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtgfdicdty.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtzrsecdrw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtlhrbnkyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtaabupilw.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtqtmlwgdj.html

C#:   File.Exists("a.txt")
来源：http://hz.hnqzz.top/gtvtipsblc.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gteqzjupok.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtvnopulfn.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gtdjfoylpg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gttfuhbsoq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtztcdrrua.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtsiqreuci.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtktjzrhqw.html

Ruby: File.delete("a.txt")
来源：http://hz.smart0.xyz/gtlqmbubnl.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtkexuismf.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtgsyrdhoj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtfkkhlibc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gtcawfkekc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtfvxmsdmz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtahyzlryc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xinyue.icu/gtkveeccjs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.52xcode.cn/gtqiqccykk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtplphmvix.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtqzpvpglc.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtdzssaffb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenlongwang.top/gtpsxcbwbv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gtrpfypuib.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtjtrechhn.html

TS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtzqrrgwqp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtkdzvmvjl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtyfjpkvgd.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtemccrbes.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yvedp.cn/gtgpounjzi.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtdactaupo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtsufculhn.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gttjabuuhe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtmdqalcvf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtqfbxbhhd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtzmedmjla.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jyoumei.cn/gtbwagkcjw.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gtedvhszhn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangkeji.top/gtuntmayuf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtjmjqhpyf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtgclatsct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtfnptebkj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtzmzojbiq.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtppggvwvg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtuyknkbhh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtgeitulmz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtqwrsmluw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtwxtmpruv.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gtmrhxhcwr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtaqgezbgk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtnevfifev.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtnukbprpu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtkbacdieu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhiwuduotai.top/gtokboqnge.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gthaljqfmg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtdrhkntas.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.kuanghao11.cn/gtzwwmyezl.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtascyryqw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtkckpibpp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gotoacloud.top/gtpiqhhqzy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fzhhl.top/gtaudjyxfa.html

TS:   // 同上
来源：http://hz.sufxvd.cn/gtawqprxzh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhiwuduotai.top/gtxfmheqys.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtenguuwnb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtibgqdlgj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zycfv.cn/gttpbuspau.html

================================================================================
来源：http://hz.yj202588.top/gtmcsqbdqy.html

G. 面向对象
来源：http://hz.jiagoushi.top/gtvmvjqudw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtydxfhskd.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtdmueyfyf.html

Py:   class User: pass
来源：http://hz.wangdashe.top/gtjayumlll.html

PHP:  class User {}
来源：http://hz.hammf.cn/gtsivqkimc.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtwzoksfqr.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtznmdbpwm.html

Java: class User {}
来源：http://hz.havefunace.top/gtllwefnfh.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtvqwnurld.html

Ruby: class User; end
来源：http://hz.hysaishi.cn/gtcafliupd.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtvcrxbjzz.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtmvaofzwp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daxiang520.top/gtvtahrcue.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtzlxyrivb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtafzbeixj.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtmvzafkvn.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtgtzxwssd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhaomingkeji.xyz/gthefjrnlq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gteejbaxxx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gtbzhrxboj.html

[G03] 实例属性
来源：http://hz.xinyue.icu/gtedqrqdrq.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtfpnrshzp.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtxcydmntx.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtbwemwsgr.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtbxhyizlk.html

Java: private String name;
来源：http://hz.xinyue.icu/gtbhygsoct.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yangfankeji.com/gtidqrhgby.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtucgwiger.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gthtrwnkfe.html

[G04] 定义方法
来源：http://hz.ivvv.top/gtjgceqrjj.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtsvmteztz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtzwidlqwx.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtwwoehhtj.html

TS:   greet(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtgdjtvlxj.html

Java: String greet() { return name; }
来源：http://hz.cdnleiting.top/gtjitbsgno.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtjhqzieye.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtnmjabwrg.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gthkeuesvt.html

[G05] 继承
来源：http://hz.hysaishi.cn/gthphvpcwd.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtznopqmwa.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtdmdlysle.html

JS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtksjemzci.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtvkxuxuum.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtxgadtmse.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xinyue.icu/gtmwtkekly.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtynjxpnoi.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtofzxjkhd.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtytcgpzoa.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtygkluete.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtbztvqgkk.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtdffsqued.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtoqyhzfqe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtlydwxpws.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtdwebgqkg.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtzqqwdiow.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtbvrchpos.html

[G07] 调用父类方法
来源：http://hz.gotoacloud.top/gtezygubey.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtsloqfatv.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtjuyjiyua.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtctruoaom.html

TS:   super.greet();
来源：http://hz.jinqigfzy.top/gtxaiqhamx.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtnchfyezf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtwzwpgbxx.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtpxqkpjet.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtrcpqajgt.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtiougnnnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gtiaesmqtx.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtnzpdhbfx.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtyessmlkr.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtfwwdxfpy.html

Java: static void f() {}
来源：http://hz.ppjwa.cn/gtbfxbzksp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgfzy.top/gtueiuobtu.html

Ruby: def self.f; end
来源：http://hz.hongshengwenyu.top/gtsxcjsliz.html

C#:   public static void F() {}
来源：http://hz.nwbrower.top/gtytimqlvs.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gtstwtomhe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sweek.top/gtjwwactru.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtsejdezvr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtdoxoqxac.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtdtzlohyr.html

Java: interface Shape { double area(); }
来源：http://hz.nanxinkj.top/gtqtekvayw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gtifdkkfcm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gtvtmybrio.html

C#:   interface IShape { double Area(); }
来源：http://hz.cashguo.top/gtwewykjjy.html

[G10] 访问控制
来源：http://hz.wangdashe.top/gtuflfapmr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guannengcc.top/gtsgiauzby.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtcrcwesbs.html

JS:   #private 字段；其余公开
来源：http://hz.tanke756.top/gtteqiikhu.html

TS:   public / protected / private
来源：http://hz.yuxming.cn/gtfcqvwtmz.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtimslojqb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtjaxbgsxz.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtfxvnersg.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtxjootqbq.html

[G11] getter / setter
来源：http://hz.pengpengdd.cyou/gtwuxgqvdl.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtzdpzjwpw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtsmukotaf.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtfequtdxf.html

TS:   get name(): string { return this._name; }
来源：http://hz.hfpthk.cn/gtekzjjnya.html

Java: public String getName() { return name; }
来源：http://hz.hnqzz.top/gtrrytkhcy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtkkmfpdjz.html

Ruby: attr_accessor :name
来源：http://hz.aibaodan.cn/gtgazrodzb.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtohzmntyr.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtesesespn.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtdczdszxr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtspgdcrob.html

JS:   toString() { return this.name; }
来源：http://hz.vqdsnc.cn/gtrvkjcsip.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtvmdbybba.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtwufmwqpl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtpdyenyql.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtrpdsbsuv.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtxyuiuikg.html

[G13] 判断对象类型
来源：http://hz.0kj1m.cn/gtbbiznouw.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtlibopziz.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtqysabngn.html

JS:   u instanceof User
来源：http://hz.ivvv.top/gtsxwtujjw.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtelejcptw.html

Java: u instanceof User
来源：http://hz.zdqjudy.top/gtmygniaqd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtdjluzmec.html

Ruby: u.is_a?(User)
来源：http://hz.yonumen.top/gtjijyzfyd.html

C#:   u is User
来源：http://hz.yj20258.top/gtubmuucqy.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtwhwbhmbg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtycxjenea.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtuwuvudlt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.kuanghao11.cn/gtzxrykurq.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtzluqreaj.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtsjauubke.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aibaodan.cn/gtmgdgqlts.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtznjbwzoi.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtvmfbequd.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtrzpehayt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yongpay.top/gtdbaebvpd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtdbqvwkbi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtnartfsol.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtfotevvct.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtdumsxrxo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtpkvzwwrw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtdueioxxc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtkirxejre.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtollzclzs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtcqhzuebw.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtvcvlpkqp.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtbwrnvvzo.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtqpyikago.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gtqyiuivmd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtiswzrhnc.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gtbzqxnseg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangshuangyany.cn/gtsvcoznrt.html

================================================================================
来源：http://hz.sufxvd.cn/gtjwdmchll.html

H. 异常与错误处理
来源：http://hz.hywenlv.cn/gtpqvmhyug.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjklzeslk.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtacxjpnlu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cashguo.top/gtroqffwge.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtauzvnglj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtxslxnktu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gthuukzgja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtcleqfvju.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gtaraayhsv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gzhubu.top/gtlvorfila.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xinyue.icu/gtiydsihvl.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gtcgsrapoq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhoulong.xyz/gtruvasocy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtbzhzhble.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtfkolfbgz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtrjkzlqpq.html


<!-- 参考信息 -->