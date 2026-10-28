代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.meibo888.top/gtfbclcgro.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangtech.top/gthdvjpzfe.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtjjwvoqwp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.iojbl.cn/gtxdodzhlg.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtkbxcmcjj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yangfankeji.com/gtestlayfl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gtduzhlaba.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtogfnvbpc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtmeppncwe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhongyouzk.top/gtgzpqtifr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtpytcacwt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gtpymwfzen.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daria6918.cn/gtwedizzyq.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtpeaiukdc.html

Py:   s.splitlines()
来源：http://hz.xinyue.icu/gtkbtwqiod.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj202588.top/gtzhkpfmyq.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtslmcxkih.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtgeuylvzl.html

Java: s.lines().toList()
来源：http://hz.sysykeji.top/gtmhknsttk.html

Go:   strings.Split(s, "\n")
来源：http://hz.yongpay.top/gtagbanvrv.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtbbbibxas.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtyzifbxxd.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtiksusiun.html

Py:   if not s:
来源：http://hz.sweek.top/gtiezhhbir.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hysaishi.cn/gtrryayjls.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtmblaftuq.html

TS:   if (s === "") {}
来源：http://hz.jianghu66.top/gtwbvbshtm.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtftchbrrc.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtsnpquyhe.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtotqsnqyg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nwbrower.top/gtugnthcol.html

[E21] 超长截断加省略号
来源：http://hz.yongpay.top/gthwwsrwlr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gtmomsdmps.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtteuakivn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtxatimgvt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtlxbfoail.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtocutxszk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jiagoushi.top/gtvvtoahky.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9152youxi.cn/gtahbqvwxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtrepiwpxy.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtmvqonjqz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gttakegwru.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.smart0.xyz/gtddegbuhz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtiqgrmjfn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtqtacnbtg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtlrgbchro.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zdqjudy.top/gtzeydhjqo.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gtgqkwesca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtsayikpao.html

================================================================================
来源：http://hz.daxiang520.top/gtiqozpzru.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtnlihwdgo.html

================================================================================
来源：http://hz.pycfn.com/gtatmjeuzb.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtcliodzea.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtlmapvrti.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ybcxt.top/gtavwqkdnd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cashguo.top/gtcokgjqmz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtifnsvufm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gttxtpwgsd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtsiodalns.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtxyjsycot.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuanzx.com/gtvgqnjllz.html

[F02] 逐行读取文件
来源：http://hz.hywenlv.cn/gtvdsrymyv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gtoborqaeu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.0kj1m.cn/gtnmsvfugj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtqjxtsztz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtiiqyeqel.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtedefeqje.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnxiangtu.top/gtseelzmcj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gttyxbinzb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ehwqpu.com/gtiypmsiya.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtxldsvhhg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtfmwcaznq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtzqkwffzx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtnkurgdhg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtdkifofrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtdyghbdze.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigufen.top/gtqsjsokmz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtrcpjrcmy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtmlhsytng.html

[F04] 追加写入文件
来源：http://hz.zycfv.cn/gtthmqvqgf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtugnkctem.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtryhgrosn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtxplhchze.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gteayxtibj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtutiwvfxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtvphxqydp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gthdqromit.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtzeyjizvi.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigfzy.top/gtwberjgcu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hammf.cn/gtcxpvzonp.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtrgkufqhj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtmwohqudf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtlgssaaqs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtsyyiorva.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtcugehcso.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinghuilouyu.cn/gtppcohfkc.html

C#:   File.Exists("a.txt")
来源：http://hz.ybcxt.top/gtxppgyzkr.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtuiiqpdio.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtywjldadg.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtvcmdxqoe.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtywjeeuzx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtxzwpcfdr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtnisscnfx.html

Go:   os.Remove("a.txt")
来源：http://hz.ehwqpu.com/gtxlacfisr.html

Ruby: File.delete("a.txt")
来源：http://hz.snrcjt.cn/gtzgrrovbs.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtudbtomhs.html

[F07] 创建目录（含多级）
来源：http://hz.ehwqpu.com/gtjwwsvemv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtvhaupmzd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jlsjyb.cn/gtxyljghjy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtzhpwffpv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtfplkbwgt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gtdeteohtj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtiaeccotq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gthzdehjsx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtzyzqvznq.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtjgoaxlhu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.dianchejie.cn/gtazllyrwr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtjcgxsqnq.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtsymkghly.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gthrxggzav.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtcjetndio.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gtwjklmmwn.html

Ruby: Dir.children("dir")
来源：http://hz.xuanzx.com/gtlejvaxld.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtjjrhehaj.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtukutcrlc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkhzgqncm.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtkmhxgypv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtzsomqfqq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtxungqotc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ivvv.top/gteiyuvwhj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtzbybpegw.html

Ruby: File.size("a.txt")
来源：http://hz.meibo888.top/gtycrdzqtj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.havefunace.top/gtixshijac.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gtxgsgpebp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtqyqbxwbc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtxtkuqzay.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtgljqalqk.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtcwuaarac.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtddqtfzfm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtzwpneyrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtwaypymcc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtvqbczogl.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gtnnppnhuh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtfsoecaxn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtababloqv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtxmjkpehn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtfyzmicib.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yangfankeji.com/gtosxxguku.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gthvjfgmaa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtbltfwknj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258.top/gtdtladmnz.html

[F12] CSV 读写
来源：http://hz.xylfe.cn/gtqzhvbgvb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yangfankeji.com/gtpddzzxtz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtntzpqsiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtoredxyqc.html

TS:   // 同上
来源：http://hz.cqqwz.cn/gtxadzwekw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtgtztoxqe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj202588.top/gthrdlzpmf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtjjtnfehq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.iojbl.cn/gtkzohyopb.html

================================================================================
来源：http://hz.guannengcc.top/gtkunqowpu.html

G. 面向对象
来源：http://hz.havefunace.top/gttsqjmlsb.html

================================================================================
来源：http://hz.fzhhl.top/gtigwvvukc.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtjvchhkab.html

Py:   class User: pass
来源：http://hz.iojbl.cn/gtzaiejafq.html

PHP:  class User {}
来源：http://hz.yueranfly.top/gtkmbzgrvl.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtukdzusfy.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtchrheqns.html

Java: class User {}
来源：http://hz.guannengcc.top/gtfmsxhbhn.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtbxmraflp.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtyavfidah.html

C#:   class User {}
来源：http://hz.redwolf501.top/gttcmtaatt.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gtjtqwabyf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtndbxvhkx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenjidiqi.icu/gtsrzqnkha.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtntkqcbhq.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtacdpteic.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydzc1.top/gtjtypkjbf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jiagoushi.top/gtaxzvpnfl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xylfe.cn/gtbrtsecju.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtmbeilmqi.html

[G03] 实例属性
来源：http://hz.tanke756.top/gtojjpazkd.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtyrrepbfa.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtrpbacfdx.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtfvhtkmyf.html

TS:   name: string = "x";
来源：http://hz.9152youxi.cn/gtcofjpzle.html

Java: private String name;
来源：http://hz.cheryme.top/gtxyhmektn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gthpipgeks.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtfrsanaxd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.snrcjt.cn/gtofifempa.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gthxrtrmxo.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gthbsaqkbd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtlazprxbb.html

JS:   greet() { return this.name; }
来源：http://hz.andypj.xyz/gteozheloo.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gtoibnadgn.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtiuvvepud.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gotoacloud.top/gtvpseojky.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtlnuzxgjx.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtgygqyhcb.html

[G05] 继承
来源：http://hz.yuxming.cn/gtrfprsvtq.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtorhgondv.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtmtzrjgkx.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtzebzizgr.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtoywohccg.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtrznlypfv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtmdhxibub.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtvzkvwiyz.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gtrmocqsrl.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtmpcwivdz.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtldwhaify.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtxwaaqbuv.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtocydtelm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtuvlqfxnd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtyltdpxev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtxthisouh.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gtvfdmovzc.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtzxjyudja.html

[G07] 调用父类方法
来源：http://hz.mhx1999.top/gtqcenwvdm.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtmvhhjkic.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtkcsjixux.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtxhobhjqx.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtbiyvjueb.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtszatybiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtsqohsezn.html

Ruby: super
来源：http://hz.xuanzx.com/gthpufikoo.html

C#:   base.Greet();
来源：http://hz.jinqigufen.top/gtizramggh.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtbxlvmapv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gtnflvqstd.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gthdavdpun.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gtjmapafba.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gtydmalouq.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtoohehbkm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hysaishi.cn/gtotgpmtbk.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtkqalktne.html

C#:   public static void F() {}
来源：http://hz.feifeiyinyue.top/gtbqucvtml.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtbtdcylez.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtkonmfeou.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangdashe.top/gthlkiqqea.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gttezvnwin.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gtycavkmgi.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtjxccjitd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gthyzbbpgp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cashguo.top/gtwcmrnnjy.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gttxeqofcn.html

[G10] 访问控制
来源：http://hz.fzhhl.top/gtubafonaa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtceetpwxx.html

PHP:  public / protected / private
来源：http://hz.yangfankeji.com/gtfqnhaibv.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtygtfsjwc.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtjriwxhmw.html

Java: public / protected / private / 默认包级
来源：http://hz.hnxiangtu.top/gtteiuvkxh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenzaomai.com/gtekbikqxp.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtblziqgvg.html

C#:   public / protected / private / internal
来源：http://hz.zhengqikj.top/gteauefiel.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gtaztxmwic.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtvsfhlbqd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtrgfqkcnk.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtrttyvepb.html

TS:   get name(): string { return this._name; }
来源：http://hz.tian-w.cn/gthznsjfms.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtccdrlbiv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtdhvchbyl.html

Ruby: attr_accessor :name
来源：http://hz.ydjk.org.cn/gterzbfeoc.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtfprymddr.html

[G12] 对象转字符串
来源：http://hz.ybcxt.top/gtmobmujdf.html

Py:   def __str__(self): return self.name
来源：http://hz.svipenyu.cn/gteglmlnvd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtevqikkxc.html

JS:   toString() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtguntnyny.html

TS:   toString(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtxptkrxkf.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtgrkchhla.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gtokiafkhw.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gttmbddwlg.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gtzeqtqllh.html

[G13] 判断对象类型
来源：http://hz.shangyingyoupin.top/gteomgmdzg.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtsejgdgli.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gtlmhwxvrv.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtkerdfjbc.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtokjvxand.html

Java: u instanceof User
来源：http://hz.vqdsnc.cn/gtvoawhjau.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtyxrxrhmq.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtdavsbvyd.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gtmgqiqsgr.html

[G14] 数据类 / record
来源：http://hz.tanke756.top/gtrytpybbf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtakzbvbyg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtkaqqlykx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtfrlggliv.html

TS:   type User = { name: string; age: number };
来源：http://hz.xziqi.cn/gthzjrkwgz.html

Java: record User(String name, int age) {}
来源：http://hz.0kj1m.cn/gtfljetfut.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtrxbwfkuc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.smart0.xyz/gtuhovvvxx.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gtwkomvpos.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gtfudrqkvw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tanke756.top/gtkwsekhsp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fengsongda.top/gtcxyywkpf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtxtqxsuky.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtsdyatyih.html

Java: enum Color { RED, GREEN }
来源：http://hz.gaohongyu789.top/gtteeooean.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.52xcode.cn/gtovhmneih.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtudqwtnzy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtsmuayphf.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtzhxotcqa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtghkkagbq.html


<!-- 参考信息 -->