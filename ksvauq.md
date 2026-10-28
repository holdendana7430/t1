代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yongpay.top/gtxttqghoj.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtotxfllcd.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtswyrexfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtwkgzhtry.html

JS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtrrlkdfdx.html

TS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gticnvhbtn.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtrihnlawo.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtijfkzmyp.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtbemwkjxs.html

C#:   s.Split('\n')
来源：http://hz.vqdsnc.cn/gtowagtzvo.html

[E20] 判断字符串是否为空
来源：http://hz.nanxinkj.top/gtbqwqedtn.html

Py:   if not s:
来源：http://hz.birdmap.top/gtscyoittp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtjzietowg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gtpemplrow.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtvjmdqmpp.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtjfrbkdbi.html

Go:   if s == "" {}
来源：http://hz.cucudq.cn/gtdlhullgm.html

Ruby: if s.empty?
来源：http://hz.fzhhl.top/gtniosewzz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtzsrabtjo.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gthpeeifmh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgfzy.top/gtimoixqkc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.smart0.xyz/gtihbndjih.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtdiqxurbh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtxjxvhjmr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtwcfwkwpz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtwawqqmck.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnqzz.top/gtuckufqnj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtxuerklpx.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtzpqbclic.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shzxlz.cn/gtqwhjwofg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtlpaqhwza.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtpguaxnuc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtojlhpgtj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuanzx.com/gtbjyzjxbu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sufxvd.cn/gtvzzcmqtg.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgfzy.top/gtufacbnur.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.9152youxi.cn/gtipfgcesg.html

================================================================================
来源：http://hz.9152youxi.cn/gtnabwkszh.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtufqlxkpp.html

================================================================================
来源：http://hz.wangdashe.top/gtcmdyempp.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gtdzqthyhe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dianchejie.cn/gtqorqqjhf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fzhhl.top/gtsqqhreoz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtjgwmbxbh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jiagoushi.top/gtsvleuohq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtrzycbaor.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtjgvvqcfq.html

Ruby: File.read("a.txt")
来源：http://hz.jianghu66.top/gtmfcizwed.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtoyoizgad.html

[F02] 逐行读取文件
来源：http://hz.xuanzx.com/gtgekglojm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtokvnodsd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtonbaoxkm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.meibo888.top/gtgjvfxklv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gthejlvosq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtaleoxqmh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtzcvlwlyj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gttgtolowj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtlblqsyjp.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gttfwyluda.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtmarkjkar.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ybcxt.top/gtthqvzfpm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtoplrqnnb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtyymbkien.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuxming.cn/gtrmnprrrk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtrgbwaukj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtcmnfzfzd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtfjroaayy.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtnlxqexci.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtkcmvhmxj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtnlcstkok.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtjhwbynva.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtyenuixeh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtqblmmlza.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtrljyuzmr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtvehzpfgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtvsvqbuwl.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gtgmfyyzlu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fengsongda.top/gtwakacoaa.html

PHP:  file_exists("a.txt");
来源：http://hz.c1oappe.top/gtzpknhdll.html

JS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtvheagbga.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtlkxgjmcn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtynhgmmkq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.andypj.xyz/gtxekmthtx.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuanzx.com/gtxmsoumgz.html

C#:   File.Exists("a.txt")
来源：http://hz.aibaodan.cn/gtpklewamk.html

[F06] 删除文件
来源：http://hz.zhixingplan.top/gtraoyixlz.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtxazpvics.html

PHP:  unlink("a.txt");
来源：http://hz.hnxiangtu.top/gtwbdzihpa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtnrcosehn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gtnwluuaju.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtouaxrmyn.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gttuvzrrlh.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gtugfsrsva.html

C#:   File.Delete("a.txt");
来源：http://hz.tian-w.cn/gtjfgfsxlz.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtxxmmptod.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gaohongyu789.top/gtetcnareb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtwczcceon.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gthsluzsrf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtemdtvcrf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cashguo.top/gtttovvjws.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtndhgbmcc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gthwiwidvt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtszndesln.html

[F08] 遍历目录
来源：http://hz.shanyushiyangtech.top/gtbklvkwpf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtwdhplptr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnxiangtu.top/gtnkykqawl.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtdfwivsgk.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtigegvdcz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gttulvpbgn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtlnnbxtov.html

Ruby: Dir.children("dir")
来源：http://hz.andypj.xyz/gtwycsdnby.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtczhqizlv.html

[F09] 获取文件大小
来源：http://hz.jqgfzy.top/gtpaevfvao.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtlbcjjxws.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtqkzqnvhw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtddprmdzu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gttfaibjbo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtcicjyeig.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sxryk.cn/gtmymionrc.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtspizseys.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gthedrzmoe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtgyfmwrle.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtzfzjyzbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gttfwvwswu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtlhztgcmr.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtljcztzho.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtvnjcnugw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dashuyun.cn/gtrfmtpteb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtuwfvwhtx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtrvnlgorb.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtnzehtgbj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtchgwumdn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtcwxunzmp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtymncrtzv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtaoiemtdm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tanke756.top/gttnfjcfqa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtibdzygkq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtgyjcgvak.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtsetllsqx.html

[F12] CSV 读写
来源：http://hz.zdqjudy.top/gthponednz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zycfv.cn/gtdoswluea.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtripbtbgh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtbiojhilv.html

TS:   // 同上
来源：http://hz.tian-w.cn/gtfsxmeked.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hywenlv.cn/gtdkfjjplr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.vqdsnc.cn/gtzffijbyj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtwxraaprd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtrfuhooeo.html

================================================================================
来源：http://hz.xuanzx.com/gtsiamvhvk.html

G. 面向对象
来源：http://hz.ydzc1.top/gtizivwnez.html

================================================================================
来源：http://hz.daxiang520.top/gtcboozeym.html

[G01] 定义类
来源：http://hz.yj202588.top/gtfqzpaacv.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gtvzltwudi.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtcirxqlcn.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtubbtptyv.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtyhvyhrkf.html

Java: class User {}
来源：http://hz.gzhubu.top/gtuclgeqwa.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtcdvmplsi.html

Ruby: class User; end
来源：http://hz.aizwys.cn/gtxrunywmt.html

C#:   class User {}
来源：http://hz.iojbl.cn/gtogcozgfg.html

[G02] 构造函数
来源：http://hz.jinqigufen.top/gtkozffloh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtlhaoacqu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gteojgsbaa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtbudxbycq.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtpxxfpvne.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gtklveblis.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.andypj.xyz/gtiyhodslt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gtstgkvqkz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigufen.top/gtalknkoxg.html

[G03] 实例属性
来源：http://hz.zhoulong.xyz/gtrfhvsldh.html

Py:   self.name = "x"
来源：http://hz.gotoacloud.top/gtshblsydp.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtuclhzeuv.html

JS:   this.name = "x";
来源：http://hz.c1oappe.top/gtlfxfxtuj.html

TS:   name: string = "x";
来源：http://hz.ydjk.org.cn/gtdssmgetu.html

Java: private String name;
来源：http://hz.nwbrower.top/gtmayjhxtr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtcimhhzks.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtvgncurxh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtmygbozzp.html

[G04] 定义方法
来源：http://hz.fengsongda.top/gtsrqnopwn.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtgdafpgzn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtcklfhaqm.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtyisprfwl.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtitrckkeu.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gtimxhzldz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zycfv.cn/gtkdzlkuyl.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtcuyozeay.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtrqubuakh.html

[G05] 继承
来源：http://hz.ydzc1.top/gtcdtpcmlw.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtuepbyeix.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtplnmqere.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtyctluhir.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtanvarpcv.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtejqbwhwl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtfniiahca.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gttadfzwvj.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gtakztpwxo.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtflgcjglt.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgfzy.top/gtaffygett.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtghboglka.html

JS:   greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtlqjtijne.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtcfvmxzih.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtldyanijw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtjcukcfbi.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtarvkhkhc.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtrjvbbeee.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtuauvjbjj.html

Py:   super().greet()
来源：http://hz.sweek.top/gtnflqrgki.html

PHP:  parent::greet();
来源：http://hz.ybcxt.top/gtvsfbtwfg.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtlayqthlx.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gtiswsfhxf.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtgkbjmfqf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtlpkcspqv.html

Ruby: super
来源：http://hz.guowangkeji.top/gtmryrwfxg.html

C#:   base.Greet();
来源：http://hz.jyoumei.cn/gtapievlcr.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtqtevaxzn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtwornfwbq.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtjsqbixmh.html

JS:   static f() {}
来源：http://hz.nanxuanxn.top/gtuuuqozkb.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtwdyrlnbi.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtxhsaildv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gzhubu.top/gtmrussdut.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtrpzfuvvn.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtdkfbxcdp.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gteheaspuh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.havefunace.top/gtfoyptkak.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtpzqvbmtd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuanzx.com/gtmonvoukc.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtgtismaft.html

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gtjaukukeb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtkjwwujlg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tanke756.top/gtohpbkapd.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtjxqzsgfi.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gtqaipmxtt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtqepslkhw.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtkyvfhoxv.html

JS:   #private 字段；其余公开
来源：http://hz.kuanghao11.cn/gtlonwbxsc.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtsukrhjkd.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtbhtzuutk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtsgiiezif.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtmdtprhui.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtokxluovr.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gteltwsoph.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtmqzuwxor.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtkdoabkmo.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtckzdmlez.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtdtsdqavg.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtwfolqnme.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gttloecgme.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gtdbbxnspo.html

C#:   public string Name { get; set; }
来源：http://hz.kuanghao11.cn/gtjqlfgvrh.html

[G12] 对象转字符串
来源：http://hz.havefunace.top/gtbedultli.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtwqerxtii.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtuujwehqk.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtdoxozznb.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtkczutsvw.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gtezshnahh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnqzz.top/gtutafzcnk.html

Ruby: def to_s; @name; end
来源：http://hz.snrcjt.cn/gtcjymfmsc.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtmylukvsr.html

[G13] 判断对象类型
来源：http://hz.cashguo.top/gtudpbqzje.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtfdpodkte.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtoknjufvg.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gtiswksrqq.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gtyxybfwtz.html

Java: u instanceof User
来源：http://hz.zhixingplan.top/gtogpbaokh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtsxsnqbqg.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtbabqbbyi.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtiydemyzu.html

[G14] 数据类 / record
来源：http://hz.kuanghao11.cn/gtroqewlky.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtgvbltnex.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtjepcppfs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pycfn.com/gtsbadptbh.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gtekzimipg.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtpcpiiebq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtfiyaoudl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gtqxqutmgt.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtuugzrudi.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtylognkip.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtvsrpepac.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gtiunuweau.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.redwolf501.top/gtdgtmpekn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtkenbnkfs.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxuanxn.top/gtouaadydr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtoxqzqiie.html

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtelpkiwlz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtndtjauxo.html

[G16] 对象转数组 / 字典
来源：http://hz.smart0.xyz/gtrzzhmjvv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtutpbprna.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtpdyifcfx.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gthxiqpadt.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtqfxejfqv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtofyspqsu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtiqidqaja.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtimvdkpks.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtjgjftaae.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgjskhmdp.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtqwlqajgd.html

================================================================================
来源：http://hz.nanxinkj.top/gthaipmdjj.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtetocgbzg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtwlnuggaz.html


<!-- 参考信息 -->