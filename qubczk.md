代发 wailian999

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtzssetsrg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuanzhike.top/gtbzhxnilq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gtuziztyyk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtzzgcuogh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtjcjltqqb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtdxaqnbxm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtinddapim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gotoacloud.top/gtchlopglb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.guowangkeji.top/gtjkxsmoek.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtapeqirmt.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtbxajyeec.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj202588.top/gtcsznafia.html

JS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtxsmydddt.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtywqxlovt.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gttiwkstpm.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtalwvcgcf.html

Ruby: s.lines
来源：http://hz.yuxming.cn/gtoltzouli.html

C#:   s.Split('\n')
来源：http://hz.hnxiangtu.top/gtztbypbaa.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gtfssfclzo.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gterixjhuv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtdmszbvuz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gtpcccdrgv.html

TS:   if (s === "") {}
来源：http://hz.nanxuanxn.top/gtysfuogld.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtbvpmkprs.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtisboclbi.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtsikjnhqj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.smart0.xyz/gtkwvedisk.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtuaknirkv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtdcfyfvem.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtrvildusv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtflvguerx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtcqprfznr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtoxzoaajo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtpchoopvc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuanzx.com/gtukhkwgsg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gtnabivcdt.html

[E22] 字节长度与字符长度
来源：http://hz.ydzc1.top/gthmsciqlg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.vqdsnc.cn/gtmmqiqnwm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtstfkzfgc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtzjlwyxgf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gttpbcqgst.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xziqi.cn/gtyeraxqsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.feifeiyinyue.top/gttnekbprz.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhengqikj.top/gtxzwrkhgl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenlongwang.top/gtdadiuoqy.html

================================================================================
来源：http://hz.ppjwa.cn/gtxxzgbtzi.html

F. 文件与目录
来源：http://hz.kuanghao11.cn/gtnrvqakmt.html

================================================================================
来源：http://hz.gotoacloud.top/gtpkoziolt.html

[F01] 读取整个文件
来源：http://hz.jinqigufen.top/gtznozluch.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhongyouzk.top/gtzaajdzqy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtfcivsgww.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gtrbodavxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtoftfxloz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtgebmgjjc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtzyltmxas.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gttqfthxsc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhijiandao.cn/gteciarhaq.html

[F02] 逐行读取文件
来源：http://hz.ivvv.top/gtmuvarqxl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gthwhewpqz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtmlshaavh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtbwkqazky.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtexgrpwdw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtuhzgtjgo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.vqdsnc.cn/gtnzmfhovz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhengqikj.top/gtpsngmlup.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jiagoushi.top/gtyuaiyfgb.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtfvrzuwzx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtgbanwsnx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtmfzlothn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtyzlzhmcq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtlqcuxnec.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gttqstrksl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.vqdsnc.cn/gtlrmkfzdd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhixingplan.top/gtedsdqawa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgfzy.top/gthsdavkdz.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gtyolxfvkb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtkfemujee.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sweek.top/gtyaxuiugk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtkrjfnfww.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtpvpfbhrs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtnzvbcutr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gtilycfdun.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guannengcc.top/gtrtfiphmp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.9152youxi.cn/gtlxwmrxss.html

[F05] 判断文件或目录是否存在
来源：http://hz.daxiang520.top/gtrmwdbyag.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtychdwpdq.html

PHP:  file_exists("a.txt");
来源：http://hz.hfpthk.cn/gttrxhgsib.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtamwmlnby.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtwrzrmmob.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtyglowgtf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtuylqqsuw.html

Ruby: File.exist?("a.txt")
来源：http://hz.guowangkeji.top/gtazzspvca.html

C#:   File.Exists("a.txt")
来源：http://hz.gotoacloud.top/gtheuhqxta.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtpniqwlwu.html

Py:   os.remove("a.txt")
来源：http://hz.nanxuanxn.top/gtsjiyeyqq.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gtwbyqbwzk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gtfjrzkwsy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtfmfdsmoh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtynbojkcs.html

Go:   os.Remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtcnbpybdo.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtpieqambo.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtvhsdhwnd.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtkjbhffrh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtvzsbiqbp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gtwfvnscoq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtzhpofphi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtlhscuapq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtrwcrrrga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gtejxiclmm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtbdxkhrna.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtlrqkhmet.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtraylogym.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtbtdhgenp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pycfn.com/gtarcjjdoc.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtktpmzrdy.html

TS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtarwonxfj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtpjsemsse.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenzaomai.com/gtkywnnjlu.html

Ruby: Dir.children("dir")
来源：http://hz.haohaochexian.top/gtfyvpavje.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangkeji.top/gtddiuqdwo.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gtzbznumsz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtpumwalpt.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtitxwozga.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtnqljfetd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtqpnywsck.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtqgziajoj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.iojbl.cn/gtbxehipdg.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtyhpkliqp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtfnufteqj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtdayhvlli.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtgsnjmrkh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258888.top/gtyzwzpktk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtqxbizlul.html

TS:   path.extname("a.txt")
来源：http://hz.gzhubu.top/gtrlnfitya.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gthrqfsjps.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtjaclzvif.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtvhvyyhrb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yongpay.top/gtfmozijkx.html

[F11] 复制与移动文件
来源：http://hz.yangfankeji.com/gtvbcptctj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtmxqqbmsm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sxryk.cn/gtfgqyggnp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtvzrerhbk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtazehjyuu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gzhubu.top/gtvxeuapog.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj202588.top/gtyhxsngeo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gthumctswn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cqqwz.cn/gtctnmvpgj.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtscfnbqzl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.0kj1m.cn/gtdwvhtcrf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gtibhusfkd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtutyydwln.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtzqyjuvfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zycfv.cn/gtgsbvzbxx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtzvsxcukb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.quarkkingdee.top/gtgqfgqgat.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtwzclhkpa.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpktnofje.html

G. 面向对象
来源：http://hz.tianlin.xyz/gtuzqavmfc.html

================================================================================
来源：http://hz.cqqwz.cn/gtipknjayq.html

[G01] 定义类
来源：http://hz.chenzaomai.com/gtpfmauqqs.html

Py:   class User: pass
来源：http://hz.dashuyun.cn/gttbqvdlye.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtzpbkwvgu.html

JS:   class User {}
来源：http://hz.ivvv.top/gtncrecrdf.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtvekrfyha.html

Java: class User {}
来源：http://hz.yuxming.cn/gtmtqrqqeu.html

Go:   type User struct { Name string }
来源：http://hz.meibo888.top/gtadsbthfq.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtfpysvcry.html

C#:   class User {}
来源：http://hz.fzhhl.top/gtfanfhtex.html

[G02] 构造函数
来源：http://hz.yj20258.top/gtnstfzjgy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hammf.cn/gtlajrgnca.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtvhbaizop.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtesgifiio.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtqybexbbg.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtswfoggsw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gtkbpzcdtr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shangyingyoupin.top/gtpsxkwsry.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gtqlbenqnk.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtftprnnds.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gtxwpdpadm.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtwmzsnjly.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtlbvxjdjq.html

TS:   name: string = "x";
来源：http://hz.shangyingyoupin.top/gtlghxudwv.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtgllhtzix.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuetiantiany.cn/gtbsvwqvaj.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtsnqqxvva.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigufen.top/gtpviiyqbb.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtqwcaiouh.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtwglrmvjx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtpnkdqdsq.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gtajyloebw.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtpfhcijmz.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtljmyrbtg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtfxngbtlk.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gtqjzdweao.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtxfptarpe.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtsuhrhnga.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtqsikaanx.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtqxkvuvmt.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtwjfzvlji.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtvefclmju.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtlrkesjhn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.birdmap.top/gtzfuutepf.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtdieaqpsf.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gteggqzoyp.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtmhtjvljx.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtizssbauj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtfksrewnn.html

JS:   greet() { return "admin"; }
来源：http://hz.yongpay.top/gtnooxtteg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtrizifxms.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtakkqycdn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhaomingkeji.xyz/gtusxbjchu.html

Ruby: def greet; "admin"; end
来源：http://hz.meibo888.top/gtghvofuey.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtmvwlxdbm.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtpnalahuq.html

Py:   super().greet()
来源：http://hz.shangyingyoupin.top/gtsctufjps.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtqzhcpysd.html

JS:   super.greet();
来源：http://hz.iojbl.cn/gtmjyturlv.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtluiaqrcj.html

Java: super.greet();
来源：http://hz.chenlongwang.top/gtmaymbtxo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gttdoljutc.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtodxtjzuy.html

C#:   base.Greet();
来源：http://hz.cucudq.cn/gtebmscgno.html

[G08] 静态方法与属性
来源：http://hz.zdqjudy.top/gtsshakjnp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtbppbdmxc.html

PHP:  public static function f() {}
来源：http://hz.yonumen.top/gtveheuspf.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gtfkrbydbh.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtdifiuqxr.html

Java: static void f() {}
来源：http://hz.cashguo.top/gtzcsdejvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guannengcc.top/gtmkcvbovh.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtqbuwjezt.html

C#:   public static void F() {}
来源：http://hz.cqqwz.cn/gtqwbbxpch.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtciwshsic.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.mhx1999.top/gtjeqlkvct.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnxiangtu.top/gtqskbnmai.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gtejveikje.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtuyegkred.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtuakmydfa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtolyxzdfp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtikxxemnj.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtanipecpf.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gttddwzgex.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtxvlqollj.html

PHP:  public / protected / private
来源：http://hz.havefunace.top/gtjrffmxee.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtximhjmzk.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtdnzmetsy.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtbywaniyf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sxryk.cn/gtkoenhila.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtwexnmhgf.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gthkbzobxo.html

[G11] getter / setter
来源：http://hz.chenzaomai.com/gtfjtbrbub.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtbnphwpiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtetrryqrg.html

JS:   get name() { return this._name; }
来源：http://hz.ivvv.top/gtpniudfol.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtqiemzodx.html

Java: public String getName() { return name; }
来源：http://hz.aibaodan.cn/gtnrnmuref.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtszynhgmt.html

Ruby: attr_accessor :name
来源：http://hz.andypj.xyz/gtsecskxjk.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtzbrknmek.html

[G12] 对象转字符串
来源：http://hz.wangdashe.top/gttsybckab.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gttqhfkumg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtjkzqvreh.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigfzy.top/gtlqqvmtwz.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtocarmjmp.html

Java: @Override public String toString() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtgvyufiqs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtmyuzaeit.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtcovzjcod.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtombuhfyq.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtchddvpjv.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtzevjutdf.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gtvgiylvbl.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtstcapvuc.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtvzvwadzv.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtqfzhfgbs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gttfzfvbac.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtchzsufku.html

C#:   u is User
来源：http://hz.shangyingyoupin.top/gtryijchzc.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtvigcbxjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtxmesfxga.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sysykeji.top/gtdgkeacyw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtqkgunzlq.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangkeji.top/gtcrlyuwvc.html

Java: record User(String name, int age) {}
来源：http://hz.jianghu66.top/gtfsbbukfj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtyjdvegvv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xylfe.cn/gtollijhix.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gttoonlvqj.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtssuthrbw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtxnlpwhum.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtvzuaedue.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sweek.top/gtipdjltoi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gttegeyriy.html

Java: enum Color { RED, GREEN }
来源：http://hz.guannengcc.top/gtvfsxnjph.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenlongwang.top/gtvsqoxnic.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gttrocvbif.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtdivibnvd.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtlknngvcu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgufenzy.top/gtppxwzxux.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtvhpvfjsb.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtfycxiqfn.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtpjvphlkf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtbjfwkret.html


<!-- 参考信息 -->