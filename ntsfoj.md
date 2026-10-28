代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtdtdpihlt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtruwkceim.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtsbcoisiz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ehwqpu.com/gtoonmpvwl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtsuzdetdi.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtyzwuzlkc.html

Py:   s.splitlines()
来源：http://hz.svipenyu.cn/gteobdvsiz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pycfn.com/gtnocwydpg.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtortmlogv.html

TS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtoeziciba.html

Java: s.lines().toList()
来源：http://hz.sufxvd.cn/gtqzzromwt.html

Go:   strings.Split(s, "\n")
来源：http://hz.yuxming.cn/gtlalakewn.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtfirgepud.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtvuasajvz.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtxsyhmwih.html

Py:   if not s:
来源：http://hz.xylfe.cn/gtcyyjeefx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtogshlmpw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtgxibgomh.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtxjcavqjb.html

Java: if (s.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtbgbmvijp.html

Go:   if s == "" {}
来源：http://hz.9152youxi.cn/gtnrzhqmjz.html

Ruby: if s.empty?
来源：http://hz.jinqigfzy.top/gttcaiqmrp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtrmfdwqof.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtmehbgpjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gtmxifscgd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtjpuoxaoy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtjxvddedv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtlqmveomb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtzabgyozv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cucudq.cn/gtcfhsfggm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnqzz.top/gtbiymdhor.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shuidangran.top/gtjcvwvamn.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gtqspcslew.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sxryk.cn/gtgykluogo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnxiangtu.top/gtosyauudg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtetvqgmca.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtjokcvymr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtvhkgeetw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aibaodan.cn/gtzewmtzmv.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gtjdlugxgj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydjk.org.cn/gtcwotfnvu.html

================================================================================
来源：http://hz.hnqzz.top/gtlimexrsk.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gtfcmzclil.html

================================================================================
来源：http://hz.cqqwz.cn/gthichagvm.html

[F01] 读取整个文件
来源：http://hz.gzhubu.top/gthgmlfwdd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tian-w.cn/gtyehbebix.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtynvxvpes.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ywan-chungtsiang.top/gtktodhafo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258.top/gtiddmrjor.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtkcqalyaz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gtgmmdaxqq.html

Ruby: File.read("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtnyxfkuff.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtlxftlmtc.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtzzptcfia.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gtmpxmptlj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtmxbuwzjj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtyjgpqoqa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtprtkxpak.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtlfolvskq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtonxhogip.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ivvv.top/gtdhpquxsx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtoykbyvop.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgufenzy.top/gtiinfgkyp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtleyfesgd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtgomdwwow.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtekpynnyi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtmueazzpe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gtybpyqvrz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cdnleiting.top/gtwzhbkhhr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gtxfmhljbg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gtczitskts.html

[F04] 追加写入文件
来源：http://hz.52xcode.cn/gtphuduzpy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtlhzeoynk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtcdffuqvq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gttupjqemf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtiwnpdffe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydjk.org.cn/gtygziypzw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinyuanbaomall.cn/gthkislycr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtrtaqawar.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtehrmtfbs.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtctuvqnlc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtdzwtzciv.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gtjrcnjqos.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtniblqwyy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtpqvbtdyp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gthrgmctay.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ywan-chungtsiang.top/gtuaonuyzi.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gtjofytpfh.html

C#:   File.Exists("a.txt")
来源：http://hz.shzxlz.cn/gttlskxbbp.html

[F06] 删除文件
来源：http://hz.havefunace.top/gtkwykiiax.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtyncadixk.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258888.top/gtyoucttvv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtemydwuam.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gthkmmoshu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtmwzxvujr.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtwddwchjx.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gtprlqtkdf.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtnvzvhasp.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtiffvqilq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtaqlsqeko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtruzaurwe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtkctctxun.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtbkyyrolm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenlongwang.top/gtwumogyld.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtthtyrxhj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtdysfhrvq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtdtewamcv.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtiznkjwxw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtduookeyz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtmhsjzvqw.html

JS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtfaeglvjk.html

TS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtazaveuil.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtxoiojidl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtglluvfhr.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtevjytnpk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigufen.top/gtvolqbeje.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtayouqywh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtmuxwgimu.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gtsrqhayug.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gtaeaapelf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtevuxafqg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtzswmblco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtyeghicen.html

Ruby: File.size("a.txt")
来源：http://hz.nanxuanxn.top/gtzsrrvrar.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aibaodan.cn/gtekwpmysj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtaxqvgmxm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtiaxflqan.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yongpay.top/gtjdtybwzm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtgybxaivh.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtpohdztzf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtsosvcxam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gttfucdpzi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtljevrrdn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.iojbl.cn/gtnyhpwjse.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtedurwvwv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtenqgsbqb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtmrmlkshr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtyqvnyiqr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtwkbgstka.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nwbrower.top/gtzuxpcjpr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gtenljivwm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtdrrnlgil.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenjidiqi.icu/gtklqxngcf.html

[F12] CSV 读写
来源：http://hz.xziqi.cn/gttbhtaemo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xylfe.cn/gtptpnafxo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gttubsppfg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtmwnzpylv.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtrumskjhb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xinyue.icu/gtgtcxlcru.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gtgqannbkt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cucudq.cn/gtqqltrmhv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tianlin.xyz/gtuenujldt.html

================================================================================
来源：http://hz.gogol.net.cn/gtsgghnjua.html

G. 面向对象
来源：http://hz.hysaishi.cn/gtvhpxadux.html

================================================================================
来源：http://hz.316326.xyz/gtywkvsoan.html

[G01] 定义类
来源：http://hz.cheryme.top/gtkioxbqnx.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtwfkwcniv.html

PHP:  class User {}
来源：http://hz.sufxvd.cn/gtlbkifljc.html

JS:   class User {}
来源：http://hz.kuanghao11.cn/gtnuvufbxm.html

TS:   class User { name: string = ""; }
来源：http://hz.shangyingyoupin.top/gtnzhfijhz.html

Java: class User {}
来源：http://hz.wangshuangyany.cn/gtpidvaodr.html

Go:   type User struct { Name string }
来源：http://hz.chenjidiqi.icu/gtzxchwsgs.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtezpsnlsl.html

C#:   class User {}
来源：http://hz.dianchejie.cn/gtyolhjfzi.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtngcdzjwc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtztuhiaxn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cdnleiting.top/gtnvktvoeh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtzymdxjfi.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gtmpvswbyb.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtpvkiglnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhiwuduotai.top/gthduungak.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtuiaqqnaf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gtsqsuntra.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtrrjxazdu.html

Py:   self.name = "x"
来源：http://hz.tanke756.top/gtrafkrntq.html

PHP:  public string $name = "x";
来源：http://hz.zhijiandao.cn/gtyzmrzauq.html

JS:   this.name = "x";
来源：http://hz.zhixingplan.top/gtiletspov.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtxryhaapc.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtocilocgc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtjvuahpyr.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gtoaqqwxgt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtcfebhzur.html

[G04] 定义方法
来源：http://hz.jinqigfzy.top/gtgqfvlurp.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gtsfrczall.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtxgxpwvpi.html

JS:   greet() { return this.name; }
来源：http://hz.zhengqikj.top/gtpkcftrsv.html

TS:   greet(): string { return this.name; }
来源：http://hz.fzhhl.top/gteqzehlnj.html

Java: String greet() { return name; }
来源：http://hz.yangfankeji.com/gtfcroratm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangdashe.top/gtsbiqiaec.html

Ruby: def greet; @name; end
来源：http://hz.gotoacloud.top/gtcmmwsinl.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtpvmmihny.html

[G05] 继承
来源：http://hz.svipenyu.cn/gttsspgdzv.html

Py:   class Admin(User): pass
来源：http://hz.ywan-chungtsiang.top/gtrtykvcrh.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtxgemghzc.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtnhbqgebg.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtwcfaegos.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtkikkwqdp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinyuanbaomall.cn/gttugefmvc.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtsgrqrlll.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtzzzdsoxb.html

[G06] 重写方法
来源：http://hz.feifeiyinyue.top/gttjpjxdsg.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangkeji.top/gtaevipuaa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtssunhhkk.html

JS:   greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtisknqoeu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gttohmmqhv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtgsztrhsl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.iojbl.cn/gteeknszft.html

Ruby: def greet; "admin"; end
来源：http://hz.ybcxt.top/gtlvuthyrm.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinyuanbaomall.cn/gtonsuwwex.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtpmdexbvo.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtlpecbajk.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtinjqfnsu.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtnrixvoco.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gtnmnlcztu.html

Java: super.greet();
来源：http://hz.jqgfzy.top/gtzxbfavzj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ppjwa.cn/gttqmqhhml.html

Ruby: super
来源：http://hz.xinyue.icu/gtqokecfnh.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gttxbilhnh.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtmvtnenjk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtvpudjemt.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gthapqvjrl.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtogflmmck.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtthpuvxoo.html

Java: static void f() {}
来源：http://hz.iojbl.cn/gtssgxmjoo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tianlin.xyz/gthrwbxihs.html

Ruby: def self.f; end
来源：http://hz.pycfn.com/gtdhvdlpox.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtlmddidvt.html

[G09] 接口 / 抽象类
来源：http://hz.yuxming.cn/gtexyatqog.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtevkqtmid.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtwnpsbikt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtnvjycgyy.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtwplomxmx.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gthxgacdkx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtsctiipdc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gttjhhcvjm.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtghezeptc.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gthaeqslxp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.haohaochexian.top/gtyrhjisbt.html

PHP:  public / protected / private
来源：http://hz.ybcxt.top/gtuxoryxbs.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtftamaids.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gthnyaybor.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gtifbgytdg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shangyingyoupin.top/gtmsgtokeg.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtdeectpgm.html

C#:   public / protected / private / internal
来源：http://hz.haohaochexian.top/gtxdssfmjc.html

[G11] getter / setter
来源：http://hz.yj20258888.top/gtaazxfayn.html

Py:   @property 与 @x.setter
来源：http://hz.9152youxi.cn/gtdffpvchd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtvollvhuf.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtixdctsps.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gtxjckkkji.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtccefrzmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnqzz.top/gtgxkixshc.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gttvxaieri.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtobtmhrxk.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtfovlmulo.html

Py:   def __str__(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtbucnbach.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtilvmviwx.html

JS:   toString() { return this.name; }
来源：http://hz.sufxvd.cn/gtsqdcdvrt.html

TS:   toString(): string { return this.name; }
来源：http://hz.316326.xyz/gtmlawkgsq.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtppbwozfs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gtrcwvsmkt.html

Ruby: def to_s; @name; end
来源：http://hz.gzhubu.top/gtseirhxug.html

C#:   public override string ToString() => Name;
来源：http://hz.yuxming.cn/gtxhtkbgfq.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gtvjvpjvez.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtjqypfnzg.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtldupbhns.html

JS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtgxrakslc.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gttzjeodmk.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtpletnpwr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtverkfirg.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtvtsyzswa.html

C#:   u is User
来源：http://hz.fengsongda.top/gtqqjmkoky.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtxrjjhqna.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtaaljndmj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtkzkalbmr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gttvhzjzlv.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtncuqhxxs.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtixgcvtuq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gtosbwespb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtzsgfiwoc.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtmwyvuklc.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gttphjluwx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtfbreqdfm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtmydgkvqg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtxcspxiha.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtwegjwgen.html

Java: enum Color { RED, GREEN }
来源：http://hz.gzhubu.top/gtavqzlbpd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gtvbqfwlrx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtoqgmmovh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtudwgskdw.html

[G16] 对象转数组 / 字典
来源：http://hz.hnxiangtu.top/gtugfltvsl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gttuxcnqsu.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gtlexuulrz.html

JS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtvmuvfmdt.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtihkybspw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtxqflyful.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtmwnqdccx.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtfwihlbhp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtnnpakepg.html

================================================================================
来源：http://hz.sxryk.cn/gtteaxbaht.html


<!-- 参考信息 -->