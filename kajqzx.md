代发 wailian999

Ruby: s.lines
来源：http://hz.xylfe.cn/gtcpuwhdak.html

C#:   s.Split('\n')
来源：http://hz.zhijiandao.cn/gtkphzhxjq.html

[E20] 判断字符串是否为空
来源：http://hz.zycfv.cn/gtfvibadnl.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtbmvehgxo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtdeyfvhuz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtajlpepqb.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtpldopovd.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gttfxbzjhf.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtvyglapcu.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtyzucmkkp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtchwsapab.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtspuxvlak.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgfzy.top/gtjjmupvcq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtctoztckl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtrxsxchni.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtbaazyvfy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gthyevgowb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtzfmstkto.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtpooohevv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sxryk.cn/gttpvzalsp.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtdwjodacn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gttawnnhen.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtcabmgwba.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtvvdavorh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtzsrecvhy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtkzrcqbbi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhoulong.xyz/gtvvrgbbqi.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtshtvnpsp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtmcpcbskl.html

================================================================================
来源：http://hz.ivvv.top/gtawfcmpdd.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtraouwnja.html

================================================================================
来源：http://hz.pycfn.com/gtwlcbyqzu.html

[F01] 读取整个文件
来源：http://hz.gzhubu.top/gteqcgztjj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgfzy.top/gtvjlhaebr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jianghu66.top/gtwdkfeotq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtrgowwqsk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtxosgfxtu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtowpuexsq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuetiantiany.cn/gtxumwvoyy.html

Ruby: File.read("a.txt")
来源：http://hz.feifeiyinyue.top/gtmqepaoiv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenzaomai.com/gtlagvahgs.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtsfvoofjs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtuqvjmdxj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dianchejie.cn/gtidqvjyde.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtpyrizyzo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gttvmpxsrj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtphchosgk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ywan-chungtsiang.top/gtvxumoium.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtwkwyiqjn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gtulgjzojp.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtagtvjkdh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtvrccqcjo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtmnkctogh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtnzckihzy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtarvnonxr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhixingplan.top/gtticyfhfx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gtlbwdtiya.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtdwdgsnbz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtkzgnmlcn.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtceziklbt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtlsemabdo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtbifbmpvo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtktwobbsv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtebwkrfzb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gtxmebptfb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtzxfpxeud.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtqfgrljoa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gtulelfzvd.html

[F05] 判断文件或目录是否存在
来源：http://hz.c1oappe.top/gttbjxodny.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gtscsumolc.html

PHP:  file_exists("a.txt");
来源：http://hz.xinyue.icu/gtdttojhfd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gthwenotgr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtbpzuyldj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtcuhtctnm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.redwolf501.top/gtcqimlwdi.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtqmwykvhs.html

C#:   File.Exists("a.txt")
来源：http://hz.zdqjudy.top/gtnlwnwbjo.html

[F06] 删除文件
来源：http://hz.nwbrower.top/gtdbeknyix.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gtffnfvzbh.html

PHP:  unlink("a.txt");
来源：http://hz.ivvv.top/gtxczlaogz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtebzeorrw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtqrmizrra.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtjekpznyp.html

Go:   os.Remove("a.txt")
来源：http://hz.cdnleiting.top/gtmgyxnnov.html

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gtuchcfjsj.html

C#:   File.Delete("a.txt");
来源：http://hz.zhongyouzk.top/gtaaardfes.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtwzdhgbjn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtpqwmvypy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.birdmap.top/gtrqbbqudq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtipoxfill.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtldkfqlsr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jiagoushi.top/gtbssswzfv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtucbccukm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sweek.top/gtkpucvcrg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gthqakbgdw.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtjzyhklfx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zdqjudy.top/gtcdhdoolk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fzhhl.top/gtgxvhmipt.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtuylvbawc.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtxhvjjzjz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtzxyvqxpq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fengsongda.top/gthmiuknvr.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtnnnrypze.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnxiangtu.top/gtmdfprtnr.html

[F09] 获取文件大小
来源：http://hz.wangshuangyany.cn/gtbxzyeeyq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tianlin.xyz/gtkfojrnco.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtcrmveonj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtgulvgprn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtrruwmfdh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gttmyjnpzn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhongyouzk.top/gtkuliglxe.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtpmoszuxu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtklpenrdu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtiaqxccbm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtdmnyuylo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtqctenify.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gthwlcoyya.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gtjjtlbopl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtqjgdtcjz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.mhx1999.top/gtrfsqcsdb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtokehrnhe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtwntzruns.html

[F11] 复制与移动文件
来源：http://hz.bjfxy.top/gtcrfeswqi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtkxekxmfg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gtoyprrwcg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gteaazblqi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtyqyrsdyu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhixingplan.top/gtponwqtkw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.kuanghao11.cn/gtuuuzplpt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtkbqpdqzn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuanzhike.top/gtvphmyvzy.html

[F12] CSV 读写
来源：http://hz.daxiang520.top/gtkmgaaaxh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtnpzhxmkt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtjchwzxzo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cashguo.top/gtesmybxsd.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtpxtjdeur.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gtxlvomogc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuanzhike.top/gtcglluoqi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtplxuwzli.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pycfn.com/gtrmomohdk.html

================================================================================
来源：http://hz.guannengcc.top/gtbcjvufmo.html

G. 面向对象
来源：http://hz.52xcode.cn/gtvdlhdntx.html

================================================================================
来源：http://hz.aibaodan.cn/gtpuzszvcs.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtekfbzqsu.html

Py:   class User: pass
来源：http://hz.birdmap.top/gtwoqgpxcm.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gthuztoyhd.html

JS:   class User {}
来源：http://hz.yonumen.top/gtjwtfffhb.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtogzwujil.html

Java: class User {}
来源：http://hz.cucudq.cn/gtgjsmgmlo.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtlfimqtpu.html

Ruby: class User; end
来源：http://hz.xziqi.cn/gteeuwjfqn.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtqlcqddqn.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gtsoydfces.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenjidiqi.icu/gtoyvggayu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtwanvbqqv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtdnzpanvg.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gteiwhmvic.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtiwlitrea.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtdykfpehg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtxsvrviwl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtdaqrrink.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtqipwelxx.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtkntmdqkk.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtnnbnxcbp.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtgjpawxub.html

TS:   name: string = "x";
来源：http://hz.yj20258888.top/gttmvqymzg.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtbkkhruef.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtlmkyirkq.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtlakehfos.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtxrprwbgz.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtmkcuxqjy.html

Py:   def greet(self): return self.name
来源：http://hz.gaohongyu789.top/gthyajkqwn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gteowzgdnv.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtdxauulmm.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtxvjthlny.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gtpfcmgbwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtjpugqixx.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtquanfybt.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtanfmiube.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtwjxvevgj.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtlfkwbxnl.html

PHP:  class Admin extends User {}
来源：http://hz.dashuyun.cn/gtcpvptpit.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtsmgrvxsh.html

TS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtxzujczof.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtgkczowke.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gteujjbszv.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gttnvmtsvj.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtnilrmuzz.html

[G06] 重写方法
来源：http://hz.daria6918.cn/gtbhswptgo.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtfkzvefvf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtgdffbbvr.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtmpruooyj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtjsgeljju.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtblyqnedw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtmutdzbmr.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtsewrqmhu.html

C#:   public override string Greet() => "admin";
来源：http://hz.cashguo.top/gtqtyvmpbm.html

[G07] 调用父类方法
来源：http://hz.zhongyouzk.top/gtxxketpen.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtuczswljn.html

PHP:  parent::greet();
来源：http://hz.gaohongyu789.top/gtkbiubdzs.html

JS:   super.greet();
来源：http://hz.dianchejie.cn/gtinqwvyox.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtdyopnvwk.html

Java: super.greet();
来源：http://hz.sysykeji.top/gttcvnonsl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxuanxn.top/gtvgwyqpdl.html

Ruby: super
来源：http://hz.mhx1999.top/gtkkgsoxcb.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtbwzcsuoq.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtgwljbpff.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtzndjxjnx.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtbgrgqjms.html

JS:   static f() {}
来源：http://hz.pycfn.com/gtpgxkmtgs.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtagcuguch.html

Java: static void f() {}
来源：http://hz.xuetiantiany.cn/gtkyswqjcc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtndpbztli.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtoiwubzqm.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gtvepascbv.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gthhohmeul.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxinkj.top/gtfsqplzea.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daxiang520.top/gtoniphljq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtiiztbfqg.html

TS:   interface Shape { area(): number; }
来源：http://hz.sweek.top/gtslwwqvol.html

Java: interface Shape { double area(); }
来源：http://hz.yangfankeji.com/gtshpkxdui.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtpaclstfv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtdorovpey.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnqzz.top/gtevudlvjt.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtzgjumvgy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtynvhrhtf.html

PHP:  public / protected / private
来源：http://hz.zhengqikj.top/gtvyczkeos.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtnrtzkchg.html

TS:   public / protected / private
来源：http://hz.daxiang520.top/gtsvtcuhdn.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtxdiapiqw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gtqrthsocz.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtjsspdxrc.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtpdjputbk.html

[G11] getter / setter
来源：http://hz.cucudq.cn/gtuqbzqbzk.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtvscrczrz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtefsfgmns.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtzuikjzmu.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gtbgygjqex.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtvnqeslam.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtfqsvlsrj.html

Ruby: attr_accessor :name
来源：http://hz.guowangkeji.top/gtzqhwwfee.html

C#:   public string Name { get; set; }
来源：http://hz.yj202588.top/gtivhxvabw.html

[G12] 对象转字符串
来源：http://hz.c1oappe.top/gtdpliffni.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtsrynxjhz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtlmwrnfew.html

JS:   toString() { return this.name; }
来源：http://hz.pycfn.com/gtzrwgkygj.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtykzlyqhm.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtsbxixuwa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnqzz.top/gtbhgrcltb.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtikpgxlmi.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtnrynvisx.html

[G13] 判断对象类型
来源：http://hz.yj20258888.top/gtzwkfdnvg.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtidfssjyt.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtbmmewifm.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtfjryuboc.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gteqgeqzab.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtbgiwwwcz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtywhrxkmc.html

Ruby: u.is_a?(User)
来源：http://hz.yj202588.top/gtuzjjorve.html

C#:   u is User
来源：http://hz.yuxming.cn/gtjzbznkdy.html

[G14] 数据类 / record
来源：http://hz.zycfv.cn/gtwvscugmv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xinyue.icu/gtbytzgfhs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtavryytgz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinghuilouyu.cn/gtqlpkzanz.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtclkkajdn.html

Java: record User(String name, int age) {}
来源：http://hz.pycfn.com/gtoitshxnm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yanxiufei.cn/gtbpthvjfm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinghuilouyu.cn/gtepjvoedy.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtdrjrnmez.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtijmtfxxb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtmormhric.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gtzrpwhfhw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtmopnwvbq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gteebcsprd.html

Java: enum Color { RED, GREEN }
来源：http://hz.yangfankeji.com/gthmkkousy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pengpengdd.cyou/gttzqcfyfh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtjsamwtqk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtwusqggxc.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtlyllldrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtwrbsalgk.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtvvctkhwf.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtadmipwgg.html

TS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gtuenxgjpg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtqbkwezti.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtzsmwyyll.html

Ruby: obj.instance_variables
来源：http://hz.sufxvd.cn/gtffwyaslm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtrglvkzvq.html

================================================================================
来源：http://hz.gogol.net.cn/gtcipozpmr.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gtefgfbopm.html

================================================================================
来源：http://hz.yvedp.cn/gtijedaeft.html

[H01] try / catch 基础
来源：http://hz.snrcjt.cn/gttpwayycd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtevxbrdqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtnubmlmkd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtktnwkvqe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gtgtgpbnvb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtegbaebbp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gtzncfurfi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtgkawfsmo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtxszllhpg.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtqtiagpre.html


<!-- 参考信息 -->