代发 wailian999

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtxyyrlnbr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtbxugwkol.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jyoumei.cn/gtzuedhvpq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtzksbcyig.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtmrulienj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yanxiufei.cn/gtvleobems.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.quarkkingdee.top/gtcnzmauya.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gtyqvwcawb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtsnkcoajj.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gthpnhjycr.html

Py:   s.splitlines()
来源：http://hz.aibaodan.cn/gtfxgeeetv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jyoumei.cn/gtgbdvpebb.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtcaomcxyx.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtigdclyph.html

Java: s.lines().toList()
来源：http://hz.xylfe.cn/gttxfohgsb.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtwiplcpsv.html

Ruby: s.lines
来源：http://hz.cqqwz.cn/gtmovyyppo.html

C#:   s.Split('\n')
来源：http://hz.mhx1999.top/gtydjiscqw.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtwaaxiehy.html

Py:   if not s:
来源：http://hz.yvedp.cn/gtljcolrik.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tian-w.cn/gtfeywjquy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zdqjudy.top/gtgnlwqest.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gttrbxxhgw.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtdhphirky.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtwmtkbjxt.html

Ruby: if s.empty?
来源：http://hz.9152youxi.cn/gthgmntatr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.havefunace.top/gtazapokwg.html

[E21] 超长截断加省略号
来源：http://hz.ydjk.org.cn/gtvxeussot.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtzyqmwirc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuanzhike.top/gtreuzauzd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtnjetxgrm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtjoxgvorz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtlcytdzxb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtvlniibdl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtdjwxaghm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtiidzyfrc.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangkeji.top/gtjzqrelue.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtrkqgydmf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtjkinchyn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtyjhmoves.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtfqivhwvp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtmfelyzvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhijiandao.cn/gtakdwekfy.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gtkhitazxx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtyxxhjidi.html

================================================================================
来源：http://hz.yonumen.top/gtautdzsqq.html

F. 文件与目录
来源：http://hz.nwbrower.top/gtpdpakypb.html

================================================================================
来源：http://hz.cucudq.cn/gtklvfvvsm.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtclhsrjiz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cashguo.top/gtnpxfudyl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtsuvxjnlr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhaomingkeji.xyz/gtzunrfoqf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtlwfwermx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtxykruphd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtdmhboiel.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtojuherbr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258888.top/gtuutgryxi.html

[F02] 逐行读取文件
来源：http://hz.sweek.top/gthljerill.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gterlydcqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cashguo.top/gtorqzeljx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtyytaaupl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtjmpyvdhr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtcrraugvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gthdftdkdm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtpfbzvtrv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtpigvtadc.html

[F03] 写入文件（覆盖）
来源：http://hz.52xcode.cn/gtcxwzxfti.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ybcxt.top/gtlakyvadx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtfwkdaruk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtqmsmzthz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtbrxatazp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtpludosny.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.feifeiyinyue.top/gtglmutjkn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ybcxt.top/gtcfpmdbes.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.c1oappe.top/gtfwbtrvkt.html

[F04] 追加写入文件
来源：http://hz.wangdashe.top/gtnhxnhsqk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtzppalqam.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtnxavjwzu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtidmwkvef.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtfnxjibeu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtoicuvdom.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnqzz.top/gtikoizeio.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtdzelacxm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gteycfubxu.html

[F05] 判断文件或目录是否存在
来源：http://hz.svipenyu.cn/gtvtckymnr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtdcflgrhj.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gttswejqti.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gthgbotpgq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtvatnqpla.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtzznlajta.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtuctmlynq.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgfzy.top/gtlsudjxry.html

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gtrxyxaniy.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtjeqqqoqh.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gthbyrelpk.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtkzdfycek.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gthdwrnuxh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtvalvmoga.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtijzhsxdh.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gtbtliadyl.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxinkj.top/gthfpivwob.html

C#:   File.Delete("a.txt");
来源：http://hz.havefunace.top/gtffvdpjfh.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtovtnexeu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtcyoqywko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dashuyun.cn/gtdwwxxfyn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtizivvhds.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtzbpveryu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gtanevqgji.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhongyouzk.top/gthkpkaitq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cheryme.top/gtbwlettss.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.0kj1m.cn/gtwselbgcs.html

[F08] 遍历目录
来源：http://hz.zhaomingkeji.xyz/gtdigmizlg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtttfbbafq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gteykfcasu.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtspkxkjhc.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtcaqfffgf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtudrshxfy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yonumen.top/gtkbccukdh.html

Ruby: Dir.children("dir")
来源：http://hz.andypj.xyz/gtqlvnocxh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhaomingkeji.xyz/gtkbppobmh.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtnmiywlpa.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtmqcfejwv.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtrjqoajnr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtufoxnuii.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtfcofjlkl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtsyucjfgv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.havefunace.top/gtkkhkdoqn.html

Ruby: File.size("a.txt")
来源：http://hz.pycfn.com/gtxnhsstur.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtplrsjvpv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gaohongyu789.top/gtkwkesods.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtqqpmaqoh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gtzqyewewi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtlwieaorc.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gtqnmokeih.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xinyue.icu/gtwrcjwdpx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtatenncvt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtpkkktfyd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dashuyun.cn/gtffkerthn.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtxgqltsdd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtmgmgjagj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtotcyozsc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtkofkklbm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtjbqwwjhs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtolybcccn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtmpcjegef.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtnkneqebj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtskejukvw.html

[F12] CSV 读写
来源：http://hz.yueranfly.top/gtyrhgvprd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gtsmlnpmox.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtjxwgzpkg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtzeynjsyp.html

TS:   // 同上
来源：http://hz.daxiang520.top/gtiteyxhsg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhixingplan.top/gtumweadod.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtelutllcy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gtqlzcqsbs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gtqokibsbs.html

================================================================================
来源：http://hz.hnxiangtu.top/gttiyyjgmp.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtlxedrmop.html

================================================================================
来源：http://hz.ydzc1.top/gtqgknwpwo.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gttpqczdjc.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtadpvmdbu.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gtzkmkfidy.html

JS:   class User {}
来源：http://hz.haohaochexian.top/gtnqlleuul.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtaozgnnri.html

Java: class User {}
来源：http://hz.wangshuangyany.cn/gtpghrmitl.html

Go:   type User struct { Name string }
来源：http://hz.cheryme.top/gtyyzuogkv.html

Ruby: class User; end
来源：http://hz.gzhubu.top/gtjkkbdvbd.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtgakkctwt.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtrkhkhxjo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zycfv.cn/gtgmmandwt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gtlphhmwgi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtkzrimlsj.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtiiwxolcz.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtkdmhfrbb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtuqiannfj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zdqjudy.top/gtiocdwfsr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtnvnwzmps.html

[G03] 实例属性
来源：http://hz.xuanzx.com/gtbibguers.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gttzwfihil.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtftvvitcq.html

JS:   this.name = "x";
来源：http://hz.ybcxt.top/gtzrsyrawf.html

TS:   name: string = "x";
来源：http://hz.shuidangran.top/gtiednipkg.html

Java: private String name;
来源：http://hz.shuidangran.top/gtsztbznuq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtyngpypir.html

Ruby: @name = "x"
来源：http://hz.zhoulong.xyz/gtrnjaufse.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gtdnztaqid.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtdanawpln.html

Py:   def greet(self): return self.name
来源：http://hz.hywenlv.cn/gtskawhafq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtfjkwqycx.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gtmstukvct.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtrjdftnpv.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtynovzoku.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xinyue.icu/gtmguskqus.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtojdihwql.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtqwamlqph.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtjrpdmpii.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtkjrgymhg.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtfkrfsxcb.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtjdaszssu.html

TS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtsihmxxwb.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtsaalbwfn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xingfuxueyuan.xyz/gtqljgwepg.html

Ruby: class Admin < User; end
来源：http://hz.sufxvd.cn/gtpbsevqfs.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gthablwtpx.html

[G06] 重写方法
来源：http://hz.yuxming.cn/gtrltocczs.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtxuicmhoy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtpzjyncow.html

JS:   greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtrskmpaws.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtjxkevupj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtqjbmiofq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gthwyyxesh.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtcrnfzroi.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtfmzsmzse.html

[G07] 调用父类方法
来源：http://hz.shangyingyoupin.top/gtmfymnhhp.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtuqqpiuac.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gttjgqztto.html

JS:   super.greet();
来源：http://hz.sweek.top/gtkhausosq.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gtlgzjnwox.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtktihylrg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gttyxhyzwa.html

Ruby: super
来源：http://hz.9152youxi.cn/gtaxmbjmmi.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtvwldpavv.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtyhivwtzr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtztpuzxvr.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtnzfqjkso.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtavsdghfs.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtmkngpxxx.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtvmvtshhp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gtmzrkyggb.html

Ruby: def self.f; end
来源：http://hz.hnqzz.top/gtghornhlv.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gteqbjvqwf.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gtwbkaxoqk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtcppyxwlj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtwdotuwth.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtgcfmnlgm.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtvmpbmpof.html

Java: interface Shape { double area(); }
来源：http://hz.jiagoushi.top/gtskkchjmw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtdwsexcin.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtagstjpiq.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtuqbbwrgy.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gtwpgqtxre.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ybcxt.top/gtqjyywqxl.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gttddutbdf.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtjuazjkfd.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gtlsdjiiau.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtdgadnaqn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.9152youxi.cn/gtjxuzidou.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gtajfmqpcg.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtrefioqwo.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtsytevlie.html

Py:   @property 与 @x.setter
来源：http://hz.jinghuilouyu.cn/gtcovarymd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtsqtybxgt.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtkswelaub.html

TS:   get name(): string { return this._name; }
来源：http://hz.tian-w.cn/gtdixxsvdg.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtvkuwrgkd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtrjvqpynd.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtmhalrmnn.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtprilbpcm.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtoqaazvmh.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtqkadlamh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtgncafbni.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtqavcaxjq.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtdjaviqxt.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtltjvwtjt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtuzmtazko.html

Ruby: def to_s; @name; end
来源：http://hz.ywan-chungtsiang.top/gtxngnqbaj.html

C#:   public override string ToString() => Name;
来源：http://hz.sxryk.cn/gtrohwvrqh.html

[G13] 判断对象类型
来源：http://hz.shzxlz.cn/gthwsfrzdy.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtpdzipzcp.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtxqxkygun.html

JS:   u instanceof User
来源：http://hz.ivvv.top/gtpldijnkw.html

TS:   u instanceof User
来源：http://hz.yj20258888.top/gtlkqhezdh.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtggzmweql.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtzttliljo.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtkalenntn.html

C#:   u is User
来源：http://hz.yongpay.top/gtfdvlduhb.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gttwvzjzyk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gteciqlnpy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtqgydlrej.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtnarbzcuv.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gttsjwnbim.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtcxrtasaq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gttzouekzr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.snrcjt.cn/gtevtecdtp.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtifwybutt.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtpccczsbr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtkmibhwav.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cqqwz.cn/gtzzdmtsby.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dashuyun.cn/gtkfaejvzd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtkgahaaii.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtmvyicbha.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtjtvdtfps.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hammf.cn/gtdvwlsqlv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtjrlwwjer.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtlydnakys.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtprsuxres.html

PHP:  get_object_vars($obj);
来源：http://hz.ybcxt.top/gtrwlmrekf.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtjqymydhv.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gttnkounky.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtjslefyec.html


<!-- 参考信息 -->