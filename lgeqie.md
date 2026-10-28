代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtkbqufupx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aizwys.cn/gttfbymqye.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtmbwohnra.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gtglutqblu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtatvigito.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtmumgsosl.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtckxlkxtq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gtcxgkpahl.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtdspswaec.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtmkxndfxb.html

Java: s.lines().toList()
来源：http://hz.haohaochexian.top/gttjozarys.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtblsbyojr.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtfjxjamvc.html

C#:   s.Split('\n')
来源：http://hz.jianghu66.top/gtrmwwgjsw.html

[E20] 判断字符串是否为空
来源：http://hz.ivvv.top/gtyiqalkwg.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gtvzjdzrpe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hongshengwenyu.top/gtbvinctrg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shuidangran.top/gtaffkjyem.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtuwlornso.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtnszzinxx.html

Go:   if s == "" {}
来源：http://hz.sweek.top/gtbearcktl.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtltcvgcfr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuanzx.com/gttevpuxrs.html

[E21] 超长截断加省略号
来源：http://hz.shangyingyoupin.top/gtfozjpmmx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtbcbuhrie.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ivvv.top/gtpzldcfha.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtavoxktgf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtohstoaqy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtcodzrurg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtvmoltisr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtgztggzez.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.svipenyu.cn/gtajrlwdmq.html

[E22] 字节长度与字符长度
来源：http://hz.xingfuxueyuan.xyz/gtsjdsmlky.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtpptccmwt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtgyufgesg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtghwfrvdv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtmyvimztx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtqbxyypbm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtmfchxlfk.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtklmigovr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtfyyqqevb.html

================================================================================
来源：http://hz.guowangkeji.top/gtabkvxxvr.html

F. 文件与目录
来源：http://hz.yueranfly.top/gtdyjesaez.html

================================================================================
来源：http://hz.9152youxi.cn/gtnrdichei.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtxsrpphrw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yonumen.top/gtskbmmpom.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtmxgrlsmr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtqtsygdbe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guannengcc.top/gtbpovpxoc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtcuistiav.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigfzy.top/gtctpayuqy.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtyagipede.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtvbvtdnhf.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtkvhdazlk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gtbtbmtziw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ywan-chungtsiang.top/gtmxtsctvg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtpwvvoqgu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtpgsdfohd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtmesowbnr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtynhuclvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenzaomai.com/gtthbqpdrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.kuanghao11.cn/gtaryxfqaa.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gtdmtoeind.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gtwwpfewmx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtobguojvj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gtmrcrotyg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtmfkfwlys.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jyoumei.cn/gtzmzrvtpe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtuhbyrkzt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtzamvizyv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daria6918.cn/gtztskcnvu.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtbhmxnuxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtplkudmjv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gtyxiyfpsf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtzbipomyz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtfgoeoeda.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xingfuxueyuan.xyz/gtwcmnjttd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guowangkeji.top/gtmvxttsmn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtmhbxafhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuetiantiany.cn/gtgmxnvohd.html

[F05] 判断文件或目录是否存在
来源：http://hz.ywan-chungtsiang.top/gtmgmtazcw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ybcxt.top/gthcyipnyu.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtfiiffyct.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtvejkdlpx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtvjxvnygm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtomghwwbo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangtech.top/gtcvwestpb.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gtuwjcfdcu.html

C#:   File.Exists("a.txt")
来源：http://hz.svipenyu.cn/gtnnsshzop.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtzltivlgt.html

Py:   os.remove("a.txt")
来源：http://hz.jianghu66.top/gtjpvwjkfy.html

PHP:  unlink("a.txt");
来源：http://hz.chenzaomai.com/gtupesspdm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtwwpnodss.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtypyvkjml.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtdyhiudhk.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gttubkkbas.html

Ruby: File.delete("a.txt")
来源：http://hz.gzhubu.top/gtzqtogire.html

C#:   File.Delete("a.txt");
来源：http://hz.cdnleiting.top/gtizvdbvcx.html

[F07] 创建目录（含多级）
来源：http://hz.guowangkeji.top/gtbbiveclf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.havefunace.top/gtcsxnrujn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dashuyun.cn/gtlebzbymy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtsubaazij.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtqqiovxyo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtkqwrhcpb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtpzdxcppd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtdlziczid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtbcihwyuc.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtsvznkvld.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtxmzyiiln.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtajpzggmf.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtouogmkdq.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtawfymbtg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtqockirnt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gthqcitttw.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtoqmlnrmq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fengsongda.top/gtxbjvyusv.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtrzbzrbej.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gtcrsvuusz.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtkukbtidh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtmfwdrtjs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtshosqibz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtqemrdsxd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.haohaochexian.top/gttepifbrn.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtlaxgknwz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenjidiqi.icu/gtxxsvtiny.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtnctglzdo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtignbjlid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtujjvcnky.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gthcgfbyic.html

TS:   path.extname("a.txt")
来源：http://hz.zhixingplan.top/gtprcmworz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gtmhyiqiam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ehwqpu.com/gtpubrueni.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtqaybtssu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jyoumei.cn/gtudbbwwai.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtofslvste.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtmfdqyeba.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtitjykwms.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtnqyofdiy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtdprmabxa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fzhhl.top/gtssujummy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtzovbwifg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtrqhzkfqs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtwifxanwe.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtklbpoeye.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangdashe.top/gtgpcntevw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jianghu66.top/gtkrswxprr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zdqjudy.top/gtifqczrba.html

TS:   // 同上
来源：http://hz.daxiang520.top/gtfjpuchfp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtwvebrboo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtsfeyvahd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtpzfrdjvl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.9152youxi.cn/gtkefaybcb.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdqusaglf.html

G. 面向对象
来源：http://hz.sweek.top/gtuewdpoal.html

================================================================================
来源：http://hz.yuxming.cn/gtgwplytqv.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gtwjmkzpch.html

Py:   class User: pass
来源：http://hz.havefunace.top/gtkagwtvyg.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtukmvkybu.html

JS:   class User {}
来源：http://hz.xylfe.cn/gttvrwcrpz.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gttlocvhie.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtiffmtjyx.html

Go:   type User struct { Name string }
来源：http://hz.yangfankeji.com/gtldtckwlv.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtsjzxszok.html

C#:   class User {}
来源：http://hz.sxryk.cn/gtchakhwyy.html

[G02] 构造函数
来源：http://hz.yuanzhike.top/gtpyyyhkfi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shangyingyoupin.top/gtokohqiaa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtgqzzybzw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cheryme.top/gtuhiiwyyt.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gtvrocnzlp.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtbsinxpuk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aibaodan.cn/gtegbhxdcf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.kuanghao11.cn/gtledjjvhv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sysykeji.top/gttboayhnm.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gteubcugjq.html

Py:   self.name = "x"
来源：http://hz.nanxuanxn.top/gteajvzlhm.html

PHP:  public string $name = "x";
来源：http://hz.fzhhl.top/gtgmbeofdh.html

JS:   this.name = "x";
来源：http://hz.cashguo.top/gtngfaykbm.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtzsgrsyfs.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtmnfnygjq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhoulong.xyz/gtdjojmcww.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtpxdmfnou.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtpifqmtco.html

[G04] 定义方法
来源：http://hz.jianghu66.top/gtolwgxnau.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gttudpvrbu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtvagowszz.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gteqfqezfy.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtwzpbchkv.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtclnbeweb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtqtxebpsq.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gttgobhkrh.html

C#:   public string Greet() => Name;
来源：http://hz.c1oappe.top/gtfrsosilr.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtzyddjcdt.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtzgchwrnf.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gtzksbbpcy.html

JS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtohvutava.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtolgxqywk.html

Java: class Admin extends User {}
来源：http://hz.pycfn.com/gtirdredne.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtjifhimgi.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtkkkwryzc.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtzxxqzkce.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtnvuwmgkl.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtljakuomk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtfzvkgzfj.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtwqmdbciq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtfidrsfmg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtwuzozvyf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hongshengwenyu.top/gtmhuomglx.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtslseubln.html

C#:   public override string Greet() => "admin";
来源：http://hz.cqqwz.cn/gtlkbjbssv.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtifxxozrr.html

Py:   super().greet()
来源：http://hz.hywenlv.cn/gtwsjbtxbq.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtdiexpzlv.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtlzckeoqi.html

TS:   super.greet();
来源：http://hz.yuxming.cn/gtdgshhlgi.html

Java: super.greet();
来源：http://hz.yonumen.top/gthyedtdsn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangkeji.top/gttderptum.html

Ruby: super
来源：http://hz.hysaishi.cn/gtpleboovd.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtqsvxbatd.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtppcitmnp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jiagoushi.top/gtywgahcar.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtfjaajpyi.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtabudnlyo.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtigbjwiln.html

Java: static void f() {}
来源：http://hz.316326.xyz/gtxwkuopqq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtkwofunnq.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtrduejgzr.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtglutozse.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gttfgjinpf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtzyhefvkd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shangyingyoupin.top/gtrtktghia.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtfjdkxdzv.html

TS:   interface Shape { area(): number; }
来源：http://hz.snrcjt.cn/gtvdrbakgc.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gteiprkive.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtafokxkyd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gotoacloud.top/gteftxuyum.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenzaomai.com/gtldllyssa.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtjhgbazqq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gtatignasi.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtpylaeluc.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtcoopkobj.html

TS:   public / protected / private
来源：http://hz.vqdsnc.cn/gtzdeqtktw.html

Java: public / protected / private / 默认包级
来源：http://hz.chenlongwang.top/gtsxxsqklr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtuzhxvuig.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtaqqfflpq.html

C#:   public / protected / private / internal
来源：http://hz.jinqigfzy.top/gtorfvybpt.html

[G11] getter / setter
来源：http://hz.quarkkingdee.top/gtybhsoivg.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gtscktlohu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtcxlswlfk.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gtfcjudtlm.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtuframixq.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtllmzlhie.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.52xcode.cn/gtuontmmjw.html

Ruby: attr_accessor :name
来源：http://hz.yonumen.top/gtotzatanu.html

C#:   public string Name { get; set; }
来源：http://hz.yvedp.cn/gtodnvnwfo.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtphetctpo.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtqxdltqif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtcuklggfh.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gtyoavptfz.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtbukdiqgy.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtgvizvaok.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtwqufxeld.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtcstmumdu.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtebejbnui.html

[G13] 判断对象类型
来源：http://hz.yonumen.top/gtygjcysxk.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtqwwogfdx.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtsfjkmnst.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtmcxlenoq.html

TS:   u instanceof User
来源：http://hz.cdnleiting.top/gtsyxsbpsv.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtxkizavxs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtrxiaskmj.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtczxnhdor.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtofwysmor.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtzsswdjiz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gtuszmqzju.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtymqrlclk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guowangkeji.top/gtpqhdajrz.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gthbgreqjp.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtlaysswnr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtpbpaforf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zycfv.cn/gtjnyjvmoe.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtiewklcqm.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtrtvfrcup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tianlin.xyz/gtdzfyaxum.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gtbemsmunq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtandkbocu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtdeapispt.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxinkj.top/gtvbywvdgu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.svipenyu.cn/gtoibezyst.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtvuoapgel.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtkkcfvima.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtzdfoarxv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtfqukfgfs.html

PHP:  get_object_vars($obj);
来源：http://hz.xuetiantiany.cn/gtkwthdwof.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtfkjgrmfq.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtjfrmjpty.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydjk.org.cn/gtlhsjktpg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtfwmrusyh.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtyvtytdxc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.haohaochexian.top/gtefkaodvy.html

================================================================================
来源：http://hz.hnqzz.top/gtrqcnsyxn.html


<!-- 参考信息 -->