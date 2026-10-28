代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.iojbl.cn/gtvfixhclt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhengqikj.top/gtsdzvsfun.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtslasufuw.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigufen.top/gtipvcmfpt.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtxwlbrsbi.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtmdpzfqtg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sxryk.cn/gtguhcdzjy.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtzwuzbbog.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fengsongda.top/gtffgeothv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtdocmqtbs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtysohccol.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtbrktlhzf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtantlyswp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtntpyshfc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtbqlubaeq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtrgyxreyq.html

[E22] 字节长度与字符长度
来源：http://hz.ybcxt.top/gthahnmakd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zdqjudy.top/gtsflyfvha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtlqkphcvb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtrzyoxbnn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtzwcuqzpq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuetiantiany.cn/gtcwhxjegh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.redwolf501.top/gtlfjoocnh.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gthcdfuwqp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daxiang520.top/gtucaqhvmw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmrjfkhdz.html

F. 文件与目录
来源：http://hz.iojbl.cn/gthfmgcfwu.html

================================================================================
来源：http://hz.cdnleiting.top/gtmcftmhcw.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gttpnmuhgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.feifeiyinyue.top/gtzfcaddll.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hammf.cn/gtpevcqgzc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtrqhdiuzt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtvcevbcjh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gthnlbedmr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtafbqlumg.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtdzstyhvd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtguuinfqx.html

[F02] 逐行读取文件
来源：http://hz.c1oappe.top/gtccxffyxs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gtsydgjouy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.meibo888.top/gttsjocexi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.meibo888.top/gtxqcuvndc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtrfojvyew.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtommndbjk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtaycdlozc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gtzqewibsk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gteuwyzpwa.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gtlzfdqman.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtztlimmqf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtrpdtpapb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtlmmprywe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtwqkjgslw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtvzcvoexx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aizwys.cn/gtpenzvvtd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtmbckjonh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtuuejodta.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtkityqdak.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtsghnwkun.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtrtftwiji.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtmjtquldw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtpmlinzni.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtkijbieym.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aizwys.cn/gthrmbwyst.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtoekzsajv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtucaltcgv.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtcecufcyg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yonumen.top/gtvpgzusob.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtusxavpaq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtghtwnzyz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtlnbcjrzj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtzjmtmtpz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtwrolwkic.html

Ruby: File.exist?("a.txt")
来源：http://hz.yueranfly.top/gtxphjopaj.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgfzy.top/gtidbelunz.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtnemgccur.html

Py:   os.remove("a.txt")
来源：http://hz.redwolf501.top/gtdququsue.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtijrwbpkm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtsgaqujwe.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtocvivqor.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtxvkqhmal.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtpsofztrg.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtnlvvqzem.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gteqzsthdy.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtxobmnjow.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigfzy.top/gtdingptrn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shzxlz.cn/gtikvbcava.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtppsmnkxo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtvqsffixk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxinkj.top/gtjncpnwbt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.quarkkingdee.top/gtmgwhextt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtxfdmxpjq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtunzabmft.html

[F08] 遍历目录
来源：http://hz.cashguo.top/gttrlhismd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenlongwang.top/gtvxqtowqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gthkystnjq.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtacyrnjfw.html

TS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtayvpydwu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtkdsajuwz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtvxfhavgl.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtzpivrtkb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtahzwggxp.html

[F09] 获取文件大小
来源：http://hz.ywan-chungtsiang.top/gtrwquxjza.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gtxebhwglh.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtstbinyip.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtqcguxhen.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gttqdafqic.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtlbibgwnb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ppjwa.cn/gtqpiuuteb.html

Ruby: File.size("a.txt")
来源：http://hz.fzhhl.top/gtbhkeuoje.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtbukeuoxi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gtwihjvfya.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtngjthhmm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yongpay.top/gtclqhuyyi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtwbicrezd.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtdjbeguno.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cdnleiting.top/gtmozykcep.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gttpowhija.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtejycsepo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.andypj.xyz/gtcmsrqbhf.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtxeombltl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtgizkqefx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hammf.cn/gtdowfgnqq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gthnkranrp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtabqvrvoz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.mhx1999.top/gtppdjlgdw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtwzifozbx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtammvjbzy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtwzvsjate.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtytrgcyjh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtkpwpibzf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtjcgccprd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtvdqayskx.html

TS:   // 同上
来源：http://hz.52xcode.cn/gtixhonoxv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gthlfkdjhc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtkwmazddm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.snrcjt.cn/gtdzdhjidn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gttmbqorwo.html

================================================================================
来源：http://hz.svipenyu.cn/gtigpflddu.html

G. 面向对象
来源：http://hz.daxiang520.top/gtaczmkaho.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqlychzgn.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtbqgxgbuy.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtekignayj.html

PHP:  class User {}
来源：http://hz.fengsongda.top/gtzegxklyt.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtydwjqscw.html

TS:   class User { name: string = ""; }
来源：http://hz.sxryk.cn/gtuurvyysy.html

Java: class User {}
来源：http://hz.tanke756.top/gtoeirpnow.html

Go:   type User struct { Name string }
来源：http://hz.gaohongyu789.top/gtexmvjwnt.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtkrjqrqfv.html

C#:   class User {}
来源：http://hz.316326.xyz/gtrtywbgdz.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtfrfnwsgo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhijiandao.cn/gtnixuzjoh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtabrbcxwm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtodpaergm.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gtnnhxolii.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtkpjesayz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.andypj.xyz/gtblbzpsis.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtwuljamef.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hammf.cn/gtgxojuaqw.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtmzvhzdab.html

Py:   self.name = "x"
来源：http://hz.hongshengwenyu.top/gttfjyrfin.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtdbdydnrk.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtxsknytft.html

TS:   name: string = "x";
来源：http://hz.tianlin.xyz/gtddfbxqsx.html

Java: private String name;
来源：http://hz.havefunace.top/gtmqmicwbq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gtrcjbqyou.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gtszqajizc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pengpengdd.cyou/gtiyemwtea.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtowgyisde.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtytgxsnsv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtappxpytb.html

JS:   greet() { return this.name; }
来源：http://hz.pycfn.com/gtccipztnr.html

TS:   greet(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gthlfdofpf.html

Java: String greet() { return name; }
来源：http://hz.nanxuanxn.top/gtahvfzzxl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtoyktpdpa.html

Ruby: def greet; @name; end
来源：http://hz.jinyuanbaomall.cn/gtsdhjgczq.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtdmscefgz.html

[G05] 继承
来源：http://hz.daria6918.cn/gtbvdwkxdd.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtstgkmzmz.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtnpnaaujo.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtuxzyzclp.html

TS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtlkgawaps.html

Java: class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gturdyrkla.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtujmnrdwn.html

Ruby: class Admin < User; end
来源：http://hz.zhengqikj.top/gtbzzjmxdg.html

C#:   class Admin : User {}
来源：http://hz.svipenyu.cn/gtpwtpfcsc.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtscoubnhb.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtsgynnaam.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtcqwnrtrb.html

JS:   greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtkkxbuhsh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtqoqdkluk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtufdfvept.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gtrydcqgfm.html

Ruby: def greet; "admin"; end
来源：http://hz.hongshengwenyu.top/gtzgklqbwr.html

C#:   public override string Greet() => "admin";
来源：http://hz.yonumen.top/gtdchlrnii.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtuvpkmrlx.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtnfhuhzdl.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtpzmzuqeg.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtfcaxozmv.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtehqrimra.html

Java: super.greet();
来源：http://hz.hammf.cn/gtpzamomyn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dashuyun.cn/gtpsjcomyx.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtchcphmky.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtawcrqspy.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtvacouvgb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtsvmswada.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtmtobopyt.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtzyewrstp.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtwhzlvswm.html

Java: static void f() {}
来源：http://hz.xylfe.cn/gtocopzada.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtysqtfwzi.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtmkseakei.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtccuysius.html

[G09] 接口 / 抽象类
来源：http://hz.yj202588.top/gtvrzokjyu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hammf.cn/gtuzrytesc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gttxmthqeo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtzbjcwqua.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnqzz.top/gttflcvdfa.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtuvhcoxyq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gthidfxouo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtxaiwornl.html

C#:   interface IShape { double Area(); }
来源：http://hz.ivvv.top/gtpsykkoki.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtukbvrxyo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258888.top/gthusntjiz.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gtpwlkprij.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtfsuofvih.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtjjiuvdtf.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtugxnspwi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gtpqeepdwm.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtjvjyoljn.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtcovpmgyg.html

[G11] getter / setter
来源：http://hz.sweek.top/gthtysbcky.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtvxeehymy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtbtmeltqs.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtomsbajuy.html

TS:   get name(): string { return this._name; }
来源：http://hz.andypj.xyz/gtfdhiizyi.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtzhxewmyt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtrdbvnjmz.html

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtnegohhpd.html

C#:   public string Name { get; set; }
来源：http://hz.daria6918.cn/gtelehtahb.html

[G12] 对象转字符串
来源：http://hz.guowangkeji.top/gtdaguwpnh.html

Py:   def __str__(self): return self.name
来源：http://hz.zdqjudy.top/gthujvwule.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtlnfllquo.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gtuyuucjid.html

TS:   toString(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtyldqfofc.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtexohiede.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenlongwang.top/gtsflncdlc.html

Ruby: def to_s; @name; end
来源：http://hz.vqdsnc.cn/gtnrotwcyw.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtirnuuxoc.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtuofzlcdl.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gthtdgykat.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtnpwevftu.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtjlmcaalc.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gtcddqoefi.html

Java: u instanceof User
来源：http://hz.pycfn.com/gtkphuigkc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.52xcode.cn/gtxmpoaehi.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtrkwdndhv.html

C#:   u is User
来源：http://hz.yvedp.cn/gtfgyhkxev.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gtcdjfxohp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtjnipqlnz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtzrptrklg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aibaodan.cn/gtonbwjrid.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtvtlkqqls.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtdeubdhgn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtjbmmuolt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shuidangran.top/gtvmjigfkz.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtyifpwgus.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtourasjil.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtncgodgxq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtdkkynzcf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pengpengdd.cyou/gtwuxjeode.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtvrpoyrar.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtohpygcyk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtpchyribh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gthxihjyxx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtrdxpqfde.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtldmjzjiu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ivvv.top/gtoymqygky.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gtaeblvilo.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gteeapyqzg.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtdbzaljxp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.316326.xyz/gtmtdwvelb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gteljnxtzq.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtivwvvrvk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtxtfrootn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdxapehzt.html

H. 异常与错误处理
来源：http://hz.tian-w.cn/gtuaagrgry.html

================================================================================
来源：http://hz.zdqjudy.top/gtjyvufqfc.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtjqcqjqcg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtsnxwvzqm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtsrfzsvwg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtosybchcm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtzjgbvacn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aibaodan.cn/gtguygkwsh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtgfaoktat.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gtehsriadg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuanzhike.top/gtemokkdil.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtbxksisxc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtenhnrgaj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtfdikyxrw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtiprlqlhf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtumnnynyu.html


<!-- 参考信息 -->