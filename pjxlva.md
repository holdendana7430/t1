代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.svipenyu.cn/gtykkgjlru.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtiuyprbgk.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gtwfssbmtc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtwcxcenhw.html

JS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtsjgffxfj.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtvzzognxq.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtfzxsacgr.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangdashe.top/gtspfowbrx.html

Ruby: s.lines
来源：http://hz.aibaodan.cn/gtmmecpsvh.html

C#:   s.Split('\n')
来源：http://hz.daria6918.cn/gtmfqwdond.html

[E20] 判断字符串是否为空
来源：http://hz.yonumen.top/gtxbufqzky.html

Py:   if not s:
来源：http://hz.jlsjyb.cn/gtwyyxvykl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtlrbmxumt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cqqwz.cn/gtytkspcpe.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtzpsygjam.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtezytpzja.html

Go:   if s == "" {}
来源：http://hz.cucudq.cn/gtywvqbglr.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtpfplkynz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.mhx1999.top/gtitbwztnb.html

[E21] 超长截断加省略号
来源：http://hz.pycfn.com/gtlepdevos.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gotoacloud.top/gtibiivqrh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gttbcexgkg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtkrnhgckx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtdyqpvgir.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtxatmsxwg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtpfdrpwxn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtollsemmj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuanzx.com/gtctebjwfo.html

[E22] 字节长度与字符长度
来源：http://hz.gzhubu.top/gtiytkbuss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gtzppieyjk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gthjjarfhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtrnuqrymm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtlbzqzrak.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gtibuqnqzn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhengqikj.top/gtiewzwadr.html

Ruby: s.bytesize;  s.length
来源：http://hz.hfpthk.cn/gtkljlqcji.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtfwsvpylr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtyzlomxly.html

F. 文件与目录
来源：http://hz.guannengcc.top/gtgxpifkbx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxjtisrro.html

[F01] 读取整个文件
来源：http://hz.yangfankeji.com/gtycqwtars.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jiagoushi.top/gtacjdxmxw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.vqdsnc.cn/gtshnxwwsc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zycfv.cn/gtcvzyawiv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gtzqdrqxnd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtzmonaeuq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtydqzqidk.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtxiedjesf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtezvymsvd.html

[F02] 逐行读取文件
来源：http://hz.ydjk.org.cn/gtieefkfvo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxuanxn.top/gtgzfrcotl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guannengcc.top/gtipsmvrav.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtpkayopxg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtqitaztyp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtqszlynns.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtihyadurj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhaomingkeji.xyz/gtccadtgmd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tian-w.cn/gtcmjpyujb.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtrraekrnl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cheryme.top/gteyziicdk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtaqpaepxs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtykesxtdp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtwtzyxyus.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtnecmpyee.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtoogrtxwm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.kuanghao11.cn/gtjwptqrxr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtuqqrrxqk.html

[F04] 追加写入文件
来源：http://hz.ivvv.top/gtglzerttb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinyuanbaomall.cn/gtrbkyjbey.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ivvv.top/gtzreioelt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtteqtqhcz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guowangkeji.top/gtkxuxckex.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuanzhike.top/gtklmucqyc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtycrgxnle.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.quarkkingdee.top/gtbucurzoe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxuanxn.top/gtzggjadwh.html

[F05] 判断文件或目录是否存在
来源：http://hz.gzhubu.top/gtpvmrwfem.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtmmbqhkux.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtdbrrbdiy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtoryhfjqv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtdevfpnvv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtjxjceuub.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtglowwuie.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenjidiqi.icu/gtilwjopvx.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtiudxdsav.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtibkvdfef.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gtltcgijqa.html

PHP:  unlink("a.txt");
来源：http://hz.ydzc1.top/gtugxmragv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtanarsmwp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtnxxseysb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtbxddriuk.html

Go:   os.Remove("a.txt")
来源：http://hz.xylfe.cn/gttjvqgbrv.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtdckcdzhi.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtdqameyos.html

[F07] 创建目录（含多级）
来源：http://hz.havefunace.top/gtdbckbdis.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtjatiepjb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtpccseqjd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtrqmitcoo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtrhjvtius.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gtjrjrrone.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dashuyun.cn/gtnmixsbqc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtcttzikbq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtjwvtwnob.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtesmmmiql.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinyuanbaomall.cn/gtcqhirxwb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zycfv.cn/gtlzjqbsfz.html

JS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtbxwfsbvi.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtphyyyelg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtbkohkbuv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuanzhike.top/gtjdjoonzf.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtaxvrtezm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.birdmap.top/gtiodkgfel.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtsezgmyxt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghu66.top/gtxzitckew.html

PHP:  filesize("a.txt");
来源：http://hz.xziqi.cn/gtvwigrhmz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtggantxvp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtculgfzah.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.birdmap.top/gttziayamk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtumwotanz.html

Ruby: File.size("a.txt")
来源：http://hz.sysykeji.top/gtotnghhhb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtvnkfeviw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gtsjulfayb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtryulpwmo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtueiqiboq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtsdnbieww.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtaaxdpzvo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtnkjeznzu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtwluwfwzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtimzxhfjp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.mhx1999.top/gtmhvxtqud.html

[F11] 复制与移动文件
来源：http://hz.shangyingyoupin.top/gtsyovhoat.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtguudksic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtxkzvihgl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtpmrqxvvn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gthqyoevnh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtwsvlhora.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hongshengwenyu.top/gtaeagfpkc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtgykyqwat.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.bjfxy.top/gtmxcvmzbn.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gtrtlzonam.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sufxvd.cn/gthwrrmcws.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gttrzdnkip.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtdrwgouvv.html

TS:   // 同上
来源：http://hz.ehwqpu.com/gtknoqixiz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtppjjyfzs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtawietjkw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtmcdefbxc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtfyyxwpnm.html

================================================================================
来源：http://hz.cqqwz.cn/gtkxgwrbbf.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtpsxuduym.html

================================================================================
来源：http://hz.tian-w.cn/gtivmeqcax.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtaujinyxn.html

Py:   class User: pass
来源：http://hz.havefunace.top/gtbcqdiwix.html

PHP:  class User {}
来源：http://hz.gogol.net.cn/gthziwjlja.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtpqkiilsn.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtnjkwyhei.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtlmksdnzr.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtsoqrmwyj.html

Ruby: class User; end
来源：http://hz.yanxiufei.cn/gtajucjusl.html

C#:   class User {}
来源：http://hz.chenlongwang.top/gtgtsftizq.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtgqoiqrbf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guannengcc.top/gtbjnywskr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gzhubu.top/gtzmonlgkq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtvdabjjbs.html

TS:   constructor(public name: string) {}
来源：http://hz.yj202588.top/gtyictgtrz.html

Java: User(String name) { this.name = name; }
来源：http://hz.sweek.top/gtijrniyzd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtzwiemwxb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.c1oappe.top/gtkuefgrzv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gtkypwqrfr.html

[G03] 实例属性
来源：http://hz.yanxiufei.cn/gtfmujhkoe.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gtcufwkwpz.html

PHP:  public string $name = "x";
来源：http://hz.yuanzhike.top/gtwcfzbpza.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gtfdjdkrfg.html

TS:   name: string = "x";
来源：http://hz.yj202588.top/gtjxtsrjbb.html

Java: private String name;
来源：http://hz.feifeiyinyue.top/gthfmsajtx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gtnujczqyi.html

Ruby: @name = "x"
来源：http://hz.mhx1999.top/gtrjrbijwu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj202588.top/gtdaoiqozg.html

[G04] 定义方法
来源：http://hz.bjfxy.top/gtqiswopuk.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtrcfwgxcf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtwcfupgls.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gticrcrjix.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258888.top/gtqkdqqyii.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtdjmajhjk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtwuxlrjzw.html

Ruby: def greet; @name; end
来源：http://hz.zycfv.cn/gtbnldwnme.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtgzlmprvi.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtwofxhbqe.html

Py:   class Admin(User): pass
来源：http://hz.cheryme.top/gthxnxntkz.html

PHP:  class Admin extends User {}
来源：http://hz.cucudq.cn/gtmeaqenkw.html

JS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtishwnfqm.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtifuzalws.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtzhdwwrcw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtuwwobkmg.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtlvhkotse.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtxvpsovpb.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtwqotwsqx.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtamjbxlgg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtsvhsabbf.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtggjctrdf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtxeduuszf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtmsczfvez.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gotoacloud.top/gtvsajoiwe.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtijtsqpmf.html

C#:   public override string Greet() => "admin";
来源：http://hz.aibaodan.cn/gtclvzytex.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtfjnyxbpy.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtshlsqtpq.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtlylvnvco.html

JS:   super.greet();
来源：http://hz.316326.xyz/gttgrjlakt.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtcmkqsmxl.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtpucjbxxl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtpsbirkzj.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtcxeuifcf.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtcqmdbqox.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtdrhsttre.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtrxqqctkv.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtotyrzgfh.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtikxfstia.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtbphntenf.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gtmlnkpwxg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtboqqwbau.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gtotqmgbox.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtuyqgjjrs.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gtpyfwqmzf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gtovkidmca.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dashuyun.cn/gtztrcxxlf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtmztzpqgx.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtcymgnyui.html

Java: interface Shape { double area(); }
来源：http://hz.smart0.xyz/gthbswrqim.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.c1oappe.top/gtckryfenh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shangyingyoupin.top/gtesdsjvyl.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangkeji.top/gtlenlenln.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gttuqrrppg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.meibo888.top/gtisezvwcz.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtoxzyotoq.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtoxozzwoc.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtvinvdfob.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gticumdsxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtnayxkyik.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtezzsadcy.html

C#:   public / protected / private / internal
来源：http://hz.yuanzhike.top/gtbveqsodv.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtfbiswosp.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtisvmhwzh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtfikfxbzn.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtnmdpnxjn.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtldgazltr.html

Java: public String getName() { return name; }
来源：http://hz.nwbrower.top/gtgwxirppr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtjlmaruvr.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gttwhkzxca.html

C#:   public string Name { get; set; }
来源：http://hz.quarkkingdee.top/gtckxarqva.html

[G12] 对象转字符串
来源：http://hz.meibo888.top/gtfyfrhzqq.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtvbqzubof.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtokbpfids.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtgijpseqz.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gtxvpzeycn.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtrqngupvq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gthjaestqr.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigufen.top/gtwuebiyor.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtfpazsaoq.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gteymohmmk.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gthhgsuwjx.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtzocymrvy.html

JS:   u instanceof User
来源：http://hz.xylfe.cn/gtilwiywxh.html

TS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtplibuvqs.html

Java: u instanceof User
来源：http://hz.meibo888.top/gttfupfrtw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtuyvqxsrp.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtbosnzgnx.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtwnoqhyjr.html

[G14] 数据类 / record
来源：http://hz.tanke756.top/gtryqlziuf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtysyumwsm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtehnjblqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtxkbgobwz.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtgdmjqqnz.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtckncawow.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtrpkksrmk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenlongwang.top/gtdaxrkazq.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtzjiqyyax.html

[G15] 枚举
来源：http://hz.sufxvd.cn/gtfqtcbegr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtjooyoxug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gtihtngxlm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtmmgcvwcn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtcibkdcnm.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtwtuszvwk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xingfuxueyuan.xyz/gtssjoekhs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shangyingyoupin.top/gtpujbiuwh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtuwwweciv.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gtuftmfcpb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtrulhvdzh.html

PHP:  get_object_vars($obj);
来源：http://hz.ydjk.org.cn/gtwdwojhwv.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtryhnnjhl.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtlllkkstu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pycfn.com/gtcnveqsdg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj202588.top/gtegamocbf.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtyfmlnctk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtxbpkckra.html

================================================================================
来源：http://hz.daria6918.cn/gtjgmhglwi.html

H. 异常与错误处理
来源：http://hz.c1oappe.top/gtklhrncll.html

================================================================================
来源：http://hz.ybcxt.top/gtavpmibwc.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtsmuotwen.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtpkbpnsmj.html


<!-- 参考信息 -->