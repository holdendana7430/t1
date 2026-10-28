代发 wailian999

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtyyvsczir.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pycfn.com/gtspfqfopv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtgziffgto.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtujepcrpu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtxpcmoebe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtpnysuqde.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gtojdgvoks.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydzc1.top/gtlruqpwru.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hysaishi.cn/gtmqxhbbpr.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtmjwqvlyq.html

Py:   s.splitlines()
来源：http://hz.jinqigufen.top/gtwproxwcp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.iojbl.cn/gtohclqzol.html

JS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtlyhojfto.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtwpnlnbki.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtgojxsyrg.html

Go:   strings.Split(s, "\n")
来源：http://hz.tian-w.cn/gtegihrjxa.html

Ruby: s.lines
来源：http://hz.zhijiandao.cn/gtysbffbut.html

C#:   s.Split('\n')
来源：http://hz.shangyingyoupin.top/gtuojzazzw.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtidswuyrh.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtdxffvszm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtejjvxnyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtnjqfyiry.html

TS:   if (s === "") {}
来源：http://hz.chenjidiqi.icu/gtxxzlspat.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtucguosvc.html

Go:   if s == "" {}
来源：http://hz.daria6918.cn/gtorwgweyf.html

Ruby: if s.empty?
来源：http://hz.wangshuangyany.cn/gtxbfdtbpa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtcdwunkes.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtrjezccug.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gtwspeibch.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtrcacyjym.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtzisehoyl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtninvrpsz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtxoibfunn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xinyue.icu/gtxrighsqd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtpxjxtsgz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtlhvnrxoc.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtxmnpxipg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gtrmovczvn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtkacmslpk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtcccrgcdr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtdsaztpcf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtjwfeyahu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtffkljkan.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgufenzy.top/gttlrhdrnq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtemusmxjh.html

================================================================================
来源：http://hz.316326.xyz/gtnhtoqbcz.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtnvrqhwpb.html

================================================================================
来源：http://hz.yuanzhike.top/gtnffhshds.html

[F01] 读取整个文件
来源：http://hz.ydzc1.top/gtqsxgfmym.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jianghu66.top/gtsmnlanof.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtxqpsclgk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gturkqiokj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuxming.cn/gtosvdkzjo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtltzsvhou.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gtljgditiq.html

Ruby: File.read("a.txt")
来源：http://hz.pycfn.com/gtxiwreyhu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtybxnhelf.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtfudpbisg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtrczvfsvi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nwbrower.top/gtdotgttju.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtggmnnumg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtyckbkmfz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtfepgjzqv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gtcjrhvktv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtpuvcoktl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hysaishi.cn/gtcrrhyzpd.html

[F03] 写入文件（覆盖）
来源：http://hz.svipenyu.cn/gtlctoudbs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtpbekoqfg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtqmtfctyx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtmlhbgous.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtfsfxqnxy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydjk.org.cn/gtpwjleqpv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shangyingyoupin.top/gtyuqcqhxu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtdqtmpldl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtynutiabq.html

[F04] 追加写入文件
来源：http://hz.yvedp.cn/gtdizmuwxk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cashguo.top/gtthynbnoc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aizwys.cn/gtxpkeisvo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtpbrtcxof.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtunznputa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtejzqwhkg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtpweavnli.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gticaqesrx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gtcyiqoras.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtsqmjzfzu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.svipenyu.cn/gtulrjyrde.html

PHP:  file_exists("a.txt");
来源：http://hz.wangdashe.top/gthqlndeaf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtomqgxkmg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtlyzejlnw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtertojmgo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.birdmap.top/gtuxwrlscc.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtoskkbmle.html

C#:   File.Exists("a.txt")
来源：http://hz.gaohongyu789.top/gthglpsudh.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtxnglsutg.html

Py:   os.remove("a.txt")
来源：http://hz.jqgfzy.top/gtriqectcw.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtmnsqdfza.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtfjnbiwyd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtygrbzftv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtcnxmafyu.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxsxsxdgd.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtgjaalgkd.html

C#:   File.Delete("a.txt");
来源：http://hz.cheryme.top/gtdnorqmos.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtatroddlz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtyozubcsx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtkgxshkvb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtquscugns.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtlkmdvpfe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtormprgkj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtdkyefiha.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtvqptgyls.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtoebpqcps.html

[F08] 遍历目录
来源：http://hz.sufxvd.cn/gtargdqosa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jianghu66.top/gtnlafnxqg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtpcxvdfwy.html

JS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtozmydhkc.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtjkwukmze.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtnhtmxjdd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtaqsdbyxl.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtxcgnntlg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gogol.net.cn/gtnrljfaqy.html

[F09] 获取文件大小
来源：http://hz.xingfuxueyuan.xyz/gtgwbrbuie.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ybcxt.top/gtylqgaguu.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtmplukiek.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtqkzfjhjs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtocqsoaev.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtrsoakjus.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ppjwa.cn/gtdvtydklo.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtriwyuiln.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtnzcxmeex.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhengqikj.top/gtcpfngsbr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtxtntlklh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dashuyun.cn/gtizqcdbat.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtxzshoiyw.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtamtierql.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nwbrower.top/gtcsgxxcjf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guannengcc.top/gthpyrysvw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtjnnbpsrn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtnjuzhado.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtxmwhwxjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtxdvwtcou.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtuqjxeejj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtjrsasgjw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gteixvcllm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtcbjcnnll.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jiagoushi.top/gthujqoztz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtkrvakedf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtygpnbjzt.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gthqrigcju.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtumtfkjah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.vqdsnc.cn/gtdzndrbof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xingfuxueyuan.xyz/gtwaeeqthi.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtoukvflye.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgufenzy.top/gtbshdygcq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtldjkkmed.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtkdfrawou.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtixnxdeph.html

================================================================================
来源：http://hz.zhixingplan.top/gtuoauzazm.html

G. 面向对象
来源：http://hz.yongpay.top/gtipvkcwgf.html

================================================================================
来源：http://hz.316326.xyz/gtswvpsiem.html

[G01] 定义类
来源：http://hz.aibaodan.cn/gtloywpmkj.html

Py:   class User: pass
来源：http://hz.gogol.net.cn/gtnvlfcjzu.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtbtlkcslb.html

JS:   class User {}
来源：http://hz.316326.xyz/gtzhillvoa.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtqlfyqpzn.html

Java: class User {}
来源：http://hz.yangfankeji.com/gtoepeuzlb.html

Go:   type User struct { Name string }
来源：http://hz.zhongyouzk.top/gtznlqevqi.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtbcppiusk.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtutkaldrg.html

[G02] 构造函数
来源：http://hz.sxryk.cn/gtscjpautm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aibaodan.cn/gtbgdygglp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangkeji.top/gtuycludmc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtuwfyqshc.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gtyycibxex.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gtgmdhzmcq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cashguo.top/gtgmclbnqv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xylfe.cn/gtblqusznm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gtpapyxxlr.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtxpopdhlu.html

Py:   self.name = "x"
来源：http://hz.gzhubu.top/gtvprqpnnd.html

PHP:  public string $name = "x";
来源：http://hz.sysykeji.top/gtxoijtqfd.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtewvijxyr.html

TS:   name: string = "x";
来源：http://hz.sweek.top/gtjftcbbli.html

Java: private String name;
来源：http://hz.sufxvd.cn/gtngjpflil.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtjrksiaay.html

Ruby: @name = "x"
来源：http://hz.zhengqikj.top/gtingpuncn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtyhodacxg.html

[G04] 定义方法
来源：http://hz.hysaishi.cn/gtlhzgcess.html

Py:   def greet(self): return self.name
来源：http://hz.yonumen.top/gtnfoqqgcs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gthmzbepdz.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtmofsebnk.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtyajgaiod.html

Java: String greet() { return name; }
来源：http://hz.chenzaomai.com/gtmpanikjq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gttvrrpclq.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gteprcyijf.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtglsaxsss.html

[G05] 继承
来源：http://hz.ivvv.top/gtbggewobb.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtcuzcgeeq.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtkzfuhvpv.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtnkqtaktp.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtuluqwclq.html

Java: class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtwcbhzxdl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtrrpomols.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtopllixej.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtaoppgjak.html

[G06] 重写方法
来源：http://hz.svipenyu.cn/gtgtdhmzyf.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtxpzkzofa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtfuvuzlke.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtwvgbwepv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtpdzpwnee.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtjrpriwyf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtmruzzmkh.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtsienvybn.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtgidwkcud.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtyxseqies.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtepiunivo.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtqdxwvxtm.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtyfkmlhtc.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtuqupqhmg.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gthysedpzq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtuglpzwzv.html

Ruby: super
来源：http://hz.52xcode.cn/gturobatnn.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtfkecezoz.html

[G08] 静态方法与属性
来源：http://hz.0kj1m.cn/gtcegmndls.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtexshfqjq.html

PHP:  public static function f() {}
来源：http://hz.yj20258888.top/gtbobjofrl.html

JS:   static f() {}
来源：http://hz.ivvv.top/gtfglbyzxm.html

TS:   static f(): void {}
来源：http://hz.haohaochexian.top/gtvpeltrkr.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtqdqinzmb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.redwolf501.top/gtcrfcvvzl.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtryuqkspd.html

C#:   public static void F() {}
来源：http://hz.yvedp.cn/gtpslocrzy.html

[G09] 接口 / 抽象类
来源：http://hz.xuanzx.com/gtpqcnbnka.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gtxsyupsqc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yongpay.top/gtisjwqrsm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtehcfrjrt.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtuueuojwy.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtbzztesif.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtwxvtaxdr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtdmotsvpy.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtbfmovana.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gthnbixgtr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gthcgbeeka.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtektnowqz.html

JS:   #private 字段；其余公开
来源：http://hz.tanke756.top/gtqjkpozrt.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtkfxtrwfq.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtrlvrgxcs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtqttewcpd.html

Ruby: public / protected / private
来源：http://hz.daxiang520.top/gttukqvnbm.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gteynnnxfy.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtelgbokoe.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtdqunmymy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtvnbhevuf.html

JS:   get name() { return this._name; }
来源：http://hz.jqgfzy.top/gtflbguuwv.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtidipfxiu.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtuueoagde.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtysbimwja.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtgkokikkc.html

C#:   public string Name { get; set; }
来源：http://hz.hysaishi.cn/gtnvdfsjjc.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtoeyjswqu.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtebobzukv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtrgmsljuh.html

JS:   toString() { return this.name; }
来源：http://hz.sweek.top/gtlseniyqz.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtpfnaiyvf.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtejavbpro.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gthbldpapd.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtvsgpzizl.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtebpyrvak.html

[G13] 判断对象类型
来源：http://hz.dianchejie.cn/gttzimkbao.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtypuhflfg.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtzihayetj.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtxkpmxbpp.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtempvuiql.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gthezdsdhu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtrrktokus.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gthpfpsldb.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtzjavmszn.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtvxrofisr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhijiandao.cn/gtfblqsdcs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtkyhxxikq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.vqdsnc.cn/gtesdzfrjs.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtblhceawc.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtgvomjres.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtdbnnkwur.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.iojbl.cn/gtwuamhkzo.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtptnzibtv.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtoqvofwhk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtylplvxph.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yanxiufei.cn/gturltnyfe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangdashe.top/gtuhktfahm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtfzxgxosb.html

Java: enum Color { RED, GREEN }
来源：http://hz.yangfankeji.com/gtgstwfnoj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhiwuduotai.top/gterdnlhdz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtjlispkvu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtutyearim.html

[G16] 对象转数组 / 字典
来源：http://hz.bjfxy.top/gtpyyjflnp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtevyhcgjo.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtvzgyuohw.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtwtndbhfv.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtaesfumvy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.quarkkingdee.top/gtimxxeirw.html


<!-- 参考信息 -->