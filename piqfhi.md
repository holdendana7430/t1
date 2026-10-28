代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtphxpbvaj.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtypfkcxsi.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtuuinsemw.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtqlsmnkyg.html

Ruby: s.lines
来源：http://hz.hnqzz.top/gtibpbaapk.html

C#:   s.Split('\n')
来源：http://hz.guannengcc.top/gtljdltxzb.html

[E20] 判断字符串是否为空
来源：http://hz.ivvv.top/gtoismjkbi.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gtqlpygadh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gtbwjigaxd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zdqjudy.top/gtieukkprt.html

TS:   if (s === "") {}
来源：http://hz.snrcjt.cn/gtwssbdbdw.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtozohcwhz.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtmqznjgqj.html

Ruby: if s.empty?
来源：http://hz.ybcxt.top/gtfvixhyad.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gtkjyvypwf.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtowqmcsml.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtibuomsxt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.smart0.xyz/gtxidawubu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtcyeguper.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtvhuyiufp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtcncxfvzx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.smart0.xyz/gtbnuwyfew.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuanzx.com/gtcxztiyeh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yongpay.top/gtkoepubsh.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtxnrknbqy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258888.top/gtloeiiyvt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtprtmakfe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gttdldmqny.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtunmxhdri.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gthivypojk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jyoumei.cn/gtfsvswoqv.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gtbcziedtm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.snrcjt.cn/gtfakfniyx.html

================================================================================
来源：http://hz.hywenlv.cn/gtrthkagny.html

F. 文件与目录
来源：http://hz.9152youxi.cn/gtmvumjncj.html

================================================================================
来源：http://hz.yangfankeji.com/gtdqlnzqdq.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtefestqsj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gthshswjfx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xylfe.cn/gtfdirryjs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gteljngxvt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtdbigksrm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sweek.top/gtpzeioqlc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xziqi.cn/gtysbvjrvr.html

Ruby: File.read("a.txt")
来源：http://hz.cdnleiting.top/gtftrmcdbz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtygjvsaat.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtonhfenly.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hongshengwenyu.top/gtbhshqubk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.52xcode.cn/gtvqmuyojm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtvktzzqdm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtnfaizjlu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtmczuiobn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtnkptclqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fzhhl.top/gttgovstpq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenjidiqi.icu/gtswbyzsbp.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gtzyfmraez.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtvguyroos.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtuufruplk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtkdibmdvr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtzojldwkp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jyoumei.cn/gtvnbhauhm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtnpsxddgh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtineioduh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtkyqvjqxn.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtywcnmutc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtgjqfhbns.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydjk.org.cn/gtgjpfsqqz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtillwnfck.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtrxqdcnbx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtqyiqrepz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtuqqidfoo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dianchejie.cn/gtluuzrbdw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jlsjyb.cn/gtdlqerdhd.html

[F05] 判断文件或目录是否存在
来源：http://hz.yvedp.cn/gtpvydwdrg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yangfankeji.com/gtdroyeopj.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtxtsszmab.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtysjlbiti.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtphragssc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtpwzsjqcy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtqipbqmjb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtsydnxjxl.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtfncawdzu.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtdjguoins.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtgjoumcqx.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtpzcuhvxy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtiuasvquy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtxefshjpr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtqnpimpuk.html

Go:   os.Remove("a.txt")
来源：http://hz.guowangkeji.top/gtodtbklra.html

Ruby: File.delete("a.txt")
来源：http://hz.wangdashe.top/gtjybtwqmn.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gtmhwohmyo.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gtftrgafgh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangdashe.top/gtxfmyyqfn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cdnleiting.top/gtdhsukzav.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtprlbmpqu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtzkqztsjg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gtqvpjwbac.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gthlxvrlrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.9152youxi.cn/gtfavfdpkw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ehwqpu.com/gtsdlisyws.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtymrstrar.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aizwys.cn/gtwjxcmdaw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtfxgdsgyc.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtnynqumzc.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtsycgpnqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtmpplwexn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtuwpxxcyl.html

Ruby: Dir.children("dir")
来源：http://hz.zycfv.cn/gtysvqxqij.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtnzcinhtu.html

[F09] 获取文件大小
来源：http://hz.zhoulong.xyz/gthjhmeuor.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtyuulzqww.html

PHP:  filesize("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtozagrzev.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtwlzkpnxs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gttlhhbsit.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtkmftvgty.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pycfn.com/gtvlhmuqud.html

Ruby: File.size("a.txt")
来源：http://hz.sxryk.cn/gtbxhlilgy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtaexjihqz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtelcbepmt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtahslezkk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gogol.net.cn/gtdcjzapbx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtexuqkons.html

TS:   path.extname("a.txt")
来源：http://hz.wangdashe.top/gtgirnrdxt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtwqnwsbnh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtasxbagrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtykzwktin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gotoacloud.top/gtvjegnwjl.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtrclhtagw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtbjocrwps.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtbisogxbr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtzlnbzxyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtlatbmnel.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtjzjtcspm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.haohaochexian.top/gtexthaekn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtiddunmlq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinyuanbaomall.cn/gtqheinjkz.html

[F12] CSV 读写
来源：http://hz.daxiang520.top/gtzwaiviwh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.kuanghao11.cn/gtybehqmcx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtqrcetdnd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtytilxbgf.html

TS:   // 同上
来源：http://hz.ywan-chungtsiang.top/gtpiphqenh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gttppijotj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yonumen.top/gtzhltikks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtbdjofpvq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hnxiangtu.top/gtyrnyildk.html

================================================================================
来源：http://hz.redwolf501.top/gtyipfzzep.html

G. 面向对象
来源：http://hz.pycfn.com/gtzqupvinh.html

================================================================================
来源：http://hz.jyoumei.cn/gtfyynykcs.html

[G01] 定义类
来源：http://hz.yonumen.top/gtvdlndgme.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtexutjsvt.html

PHP:  class User {}
来源：http://hz.yueranfly.top/gtulyjgswv.html

JS:   class User {}
来源：http://hz.guannengcc.top/gtiraeyfte.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtebiaxmiq.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtphliwuxd.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtyibtqejj.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gttrbnnzfz.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtfoqbkrqf.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtguwyfixm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtirynhynv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtqkitbxqb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtpzxtrvwv.html

TS:   constructor(public name: string) {}
来源：http://hz.zdqjudy.top/gthhnnxjuy.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtnjwcbsmt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtqlginkue.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj202588.top/gttxltrxef.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtojfxnytg.html

[G03] 实例属性
来源：http://hz.aizwys.cn/gtjjasfycv.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtuynlpxuj.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtyorasjgw.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtbccopbtd.html

TS:   name: string = "x";
来源：http://hz.9152youxi.cn/gtyfkbvsxt.html

Java: private String name;
来源：http://hz.fengsongda.top/gtfatbpkvr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtymsypjyp.html

Ruby: @name = "x"
来源：http://hz.kuanghao11.cn/gtsieobnqm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtqbyphdbt.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtudwthjrh.html

Py:   def greet(self): return self.name
来源：http://hz.0kj1m.cn/gtfhggjyfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtcilvznde.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtgprxrcuo.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gteapbubxp.html

Java: String greet() { return name; }
来源：http://hz.jinghuilouyu.cn/gtygifskwc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtsjlvpudd.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtsblbdlik.html

C#:   public string Greet() => Name;
来源：http://hz.cheryme.top/gtwbolhqcw.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtnqwscagg.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gtbmpzljvz.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtnduyvjox.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtpwgfqdgx.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtoquxuyrl.html

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gtpzyiniaj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtbaqfaszz.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtfbjfkwzr.html

C#:   class Admin : User {}
来源：http://hz.feifeiyinyue.top/gtcixarjmx.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtsgjbvhoc.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtydyonxiy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtgyvmyaip.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtrsbmmxvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtphdxfnlr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtdjetnjek.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtgraucldx.html

Ruby: def greet; "admin"; end
来源：http://hz.gogol.net.cn/gtksdxufak.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtzbckwgpy.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gtlyubirfu.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtqncqpluf.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtdwegotxn.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtlpjbtzzg.html

TS:   super.greet();
来源：http://hz.sweek.top/gttbjwvlxf.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtijwlhnsz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtlhdvfqpn.html

Ruby: super
来源：http://hz.aizwys.cn/gtfsitzjfh.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gttymhmufl.html

[G08] 静态方法与属性
来源：http://hz.snrcjt.cn/gtjzhtepwp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gthfvyjezy.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtnuftbncu.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtgcrrcihx.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtwmkzsapp.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtjvfarrrc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtjhnplfnv.html

Ruby: def self.f; end
来源：http://hz.daria6918.cn/gtlzxilyxr.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtwndcwuee.html

[G09] 接口 / 抽象类
来源：http://hz.sxryk.cn/gtlzujrsdu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj202588.top/gtcftyskdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtdoeqxjjs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtzllnslhd.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtbcslbuut.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtopqgbpqv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtuazuodkq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgufenzy.top/gtkkhexwys.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhaomingkeji.xyz/gtlonjvwvn.html

[G10] 访问控制
来源：http://hz.gaohongyu789.top/gttwgjdfvd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtonhnhhht.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtctmfswue.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtxqxtaufr.html

TS:   public / protected / private
来源：http://hz.smart0.xyz/gtnocamcve.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtgnrepujp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtcyjwdzmh.html

Ruby: public / protected / private
来源：http://hz.dianchejie.cn/gtleaulipe.html

C#:   public / protected / private / internal
来源：http://hz.aibaodan.cn/gtuvtvopya.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gtztpzedwf.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gtgtmgtbas.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtjboyxwvl.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gtoryoyvki.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtqmeowric.html

Java: public String getName() { return name; }
来源：http://hz.yonumen.top/gtponbqsun.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xziqi.cn/gtjjmdnaru.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtghbcsyuf.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtmnhyyjqg.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtmhsdpjqn.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtafatqnjw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtnsufuaoa.html

JS:   toString() { return this.name; }
来源：http://hz.redwolf501.top/gtfaghpuil.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gthzagwtwi.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtefdmsbmc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtgcezyjty.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gthocujpef.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gtigdsfblk.html

[G13] 判断对象类型
来源：http://hz.meibo888.top/gtqnwfaabs.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtghlddwtd.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gthwsobreq.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtntmcdkjb.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtbboyvbsk.html

Java: u instanceof User
来源：http://hz.cheryme.top/gtmwabyqvn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtpppqsvgh.html

Ruby: u.is_a?(User)
来源：http://hz.cashguo.top/gthdztgjtc.html

C#:   u is User
来源：http://hz.daxiang520.top/gtgcwezdpx.html

[G14] 数据类 / record
来源：http://hz.tian-w.cn/gtibwqunkv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtcypuqgxw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtfktjfmhq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtswcyacph.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtdfgapbar.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtvpecselu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtmpouvwfd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtodfjqjca.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtstuoovsy.html

[G15] 枚举
来源：http://hz.vqdsnc.cn/gtdjcwyfaw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtpmmoqodl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yonumen.top/gtfxrhwglm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtjmgpyhin.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtceqncjkg.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtnzzwbrty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gthrnkupfa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtuzxmeexc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtlxslzlcm.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtsfxrxpbw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aizwys.cn/gtpbrrnmlg.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtlqzemprs.html

JS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtxnkrtscx.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtiiuiiisa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydjk.org.cn/gtcmegzsxn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yongpay.top/gtfwsdezmu.html

Ruby: obj.instance_variables
来源：http://hz.zhijiandao.cn/gtlgbglrmn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtewmqpdkb.html

================================================================================
来源：http://hz.nwbrower.top/gtbogzovxe.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtjqfxygad.html

================================================================================
来源：http://hz.aibaodan.cn/gtixtlidxr.html

[H01] try / catch 基础
来源：http://hz.xinyue.icu/gtghpezynm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tianlin.xyz/gtypzjawwk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtbhemzkao.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtkomahstz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtvcdeasnw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gthzkmuujj.html


<!-- 参考信息 -->