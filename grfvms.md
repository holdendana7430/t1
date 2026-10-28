代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pengpengdd.cyou/gtfwtrumyc.html

[E19] 多行文本按行拆分
来源：http://hz.andypj.xyz/gttijhtrbw.html

Py:   s.splitlines()
来源：http://hz.shzxlz.cn/gtumnqqybq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zycfv.cn/gtjdosxtys.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtneaghnii.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtzpybakot.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtgjwfcdvs.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtpormbsus.html

Ruby: s.lines
来源：http://hz.jianghu66.top/gtapcxkhye.html

C#:   s.Split('\n')
来源：http://hz.316326.xyz/gtwpncqigy.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtvdtmqglz.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtsblfdflp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuanzhike.top/gtasawpbov.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daxiang520.top/gtrdkgsbkn.html

TS:   if (s === "") {}
来源：http://hz.gzhubu.top/gtbhebhdyd.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtifvdkpho.html

Go:   if s == "" {}
来源：http://hz.zhixingplan.top/gtungrtwcr.html

Ruby: if s.empty?
来源：http://hz.hnxiangtu.top/gtfsjpednh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtbjhtmmww.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtaauatvxc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtbrwzfbko.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gteospiodg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtogutmdrm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtakzrtfpu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtzbstuvrn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yangfankeji.com/gtjyajxizw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtsleqkbql.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtxwepgcpt.html

[E22] 字节长度与字符长度
来源：http://hz.guowangkeji.top/gtelrflbwk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnxiangtu.top/gtgjgqihcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtbqrocuhx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtypfdbghv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtyagvtrsa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtyxhiovxn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pengpengdd.cyou/gtsadvlzcx.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxinkj.top/gtkcccqtdv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhijiandao.cn/gtjvlqzzht.html

================================================================================
来源：http://hz.svipenyu.cn/gtcvajcwcw.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtfyqxodqy.html

================================================================================
来源：http://hz.zdqjudy.top/gtfnamsifc.html

[F01] 读取整个文件
来源：http://hz.gogol.net.cn/gtyqzcqgrg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhaomingkeji.xyz/gtugcuacxn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtllzrwqjw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtqlvoripq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gtnjmcrkbm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtkwxluunf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtiimwkzna.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigfzy.top/gtfhbvtlon.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj202588.top/gtkhnxhkgo.html

[F02] 逐行读取文件
来源：http://hz.sweek.top/gtuyqpsblv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnqzz.top/gtjdybaeaa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtkkjgrblk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtelavccwn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtjsnlqqas.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gttmanonfw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtfhrrthws.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtiyasfhcg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtjysboiem.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtdldqkmme.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtmukvjkzd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtdohttvbr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtudzpxmxg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtzmmyxrem.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtrczvuhly.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ywan-chungtsiang.top/gthuudbabo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cucudq.cn/gtrwvsdkiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.andypj.xyz/gtmkhgiofz.html

[F04] 追加写入文件
来源：http://hz.hnqzz.top/gtciyaimdd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtkbvphipp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangtech.top/gtpjwutkzr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtfrputzss.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtnuqjqkey.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.haohaochexian.top/gtvomnnylu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtckkthrfc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.vqdsnc.cn/gtxlzurosu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cashguo.top/gtxqyjvepb.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gthkgpcgog.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gteqjtpnmj.html

PHP:  file_exists("a.txt");
来源：http://hz.nwbrower.top/gtptqadtle.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtmqgiahxo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtfwquovre.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtmqedzflf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtokildqtq.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gttkmhkshq.html

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gtbnrrmytr.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtjxprygck.html

Py:   os.remove("a.txt")
来源：http://hz.birdmap.top/gtyvgptcvu.html

PHP:  unlink("a.txt");
来源：http://hz.zdqjudy.top/gtopgaqzaj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtrvibjpag.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gthdqdpoho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtmsadfbnn.html

Go:   os.Remove("a.txt")
来源：http://hz.jianghu66.top/gtkovfqiex.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtgbplmbnb.html

C#:   File.Delete("a.txt");
来源：http://hz.cdnleiting.top/gtnywmdvsv.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtyxcsovad.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtsxjfwoze.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtzdlgnrig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtzqefsowc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtppkzajlj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gttnyzupso.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cqqwz.cn/gtjhbrxoab.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yangfankeji.com/gtrbtbvrkv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yanxiufei.cn/gtuvpacxpa.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtusloicsm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtndoygopg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gttqquhywf.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtkofrlgwo.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtfhtpyjfw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtgxjwuqqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtpuaplfhk.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtqbkwpbso.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yvedp.cn/gtzgvhtehb.html

[F09] 获取文件大小
来源：http://hz.jinghuilouyu.cn/gtjwhrfgzv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuxming.cn/gtglqzmgcr.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtvhmcxqyy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gttpjehwhu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtrlpmchvt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gttidqoymy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigufen.top/gthwibrlfy.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gtgrfbdxgq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtqnzrhrfz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.meibo888.top/gtreogbnle.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtikxtsjuf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangdashe.top/gtrnavtgfs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtcfbqkkxx.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtkqhuohze.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtenwmsdkp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtnpibqouf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtuahetcvt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cqqwz.cn/gtbippmwra.html

[F11] 复制与移动文件
来源：http://hz.sufxvd.cn/gttqpyihfl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtzmzxaoxd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtqmhrwdlh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtxymvdrmo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtljqgvcqo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gogol.net.cn/gtijwlwxwz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtluvecpdz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gtvqnrngxf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gtbwrelkkx.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gthkveiura.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtnmpdddpd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gthmuelqau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtzljiwlco.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtzwlqaddt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtrslpcphe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtktcmwzgg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtcxihpnnk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtozeakthk.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvzphpwyl.html

G. 面向对象
来源：http://hz.52xcode.cn/gtibousoji.html

================================================================================
来源：http://hz.yanxiufei.cn/gttilpivad.html

[G01] 定义类
来源：http://hz.hongshengwenyu.top/gtyviwifeg.html

Py:   class User: pass
来源：http://hz.ybcxt.top/gteggqzlfw.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtcdevqlij.html

JS:   class User {}
来源：http://hz.gzhubu.top/gtxamwrtsn.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtylydvjgf.html

Java: class User {}
来源：http://hz.sysykeji.top/gtlatbahvg.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtcefggusp.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtqwvazafn.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gttkkpqpud.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtuwjzndvs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtopmltknm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gtpnstprfe.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtdnlqzrpd.html

TS:   constructor(public name: string) {}
来源：http://hz.sxryk.cn/gtapcuvrvv.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtebcwfxno.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gtlcorhthh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtnmdirass.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtffkzyexo.html

[G03] 实例属性
来源：http://hz.yj20258.top/gtwzxvnddu.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtbyeqmkkw.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gtrbxmzekq.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtchcjcxfz.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtyrlctlbm.html

Java: private String name;
来源：http://hz.sxryk.cn/gtfoufooqm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtsxzcmuja.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtbewyxwvj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuetiantiany.cn/gtexjuwqes.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gtxwhniukv.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtjbhvgmlo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtdfxyvxfq.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtxvduhafn.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtsoyzfuxx.html

Java: String greet() { return name; }
来源：http://hz.hywenlv.cn/gttfmbnmoy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtjvjktogx.html

Ruby: def greet; @name; end
来源：http://hz.shangyingyoupin.top/gtmmcgdcai.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gttjrucoae.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtyvbxmxcp.html

Py:   class Admin(User): pass
来源：http://hz.hongshengwenyu.top/gtdsmknydh.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gtwqzwsyjl.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtroctcsaw.html

TS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtiqidxeeb.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtqxvlrsrm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xinyue.icu/gtpzdturww.html

Ruby: class Admin < User; end
来源：http://hz.0kj1m.cn/gtopkrelqb.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtpelnxdih.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtwajljpcf.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258.top/gtiwrsieol.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtmbfgfddv.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtccpldbzf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtcqhdhesq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtpztczphw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtstwuqefn.html

Ruby: def greet; "admin"; end
来源：http://hz.ppjwa.cn/gtthpzpslk.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtxcaoiyfq.html

[G07] 调用父类方法
来源：http://hz.ydjk.org.cn/gtiinsggmq.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtyqlyaazq.html

PHP:  parent::greet();
来源：http://hz.cucudq.cn/gtbyfyprsi.html

JS:   super.greet();
来源：http://hz.yangfankeji.com/gtbdablsxg.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtpadwnksx.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtsidwnhds.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtjxgfulmr.html

Ruby: super
来源：http://hz.fengsongda.top/gtaakblwhf.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtknujxoxf.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gtxlivlott.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gaohongyu789.top/gtghshckha.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtfzofafsv.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtokcircxl.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtuexurwbd.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtlhtsmnbs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tianlin.xyz/gtvndrreay.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtknejkdih.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gthevsxnfp.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtqckzibww.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtdxqdrwyp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gtrseryksr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtacqgeayl.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgufenzy.top/gtmlzaennn.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtduzgqhst.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hfpthk.cn/gtnkwznyot.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtstjujwnw.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtfqxrljpc.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtwrjdbizq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtjrxuwnjb.html

PHP:  public / protected / private
来源：http://hz.jinghuilouyu.cn/gtocthgqol.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gtukflzfmy.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtdytzyote.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtxtegueax.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtggjcavxw.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtaxsaawic.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gtttzmtcbi.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtbkgshiho.html

Py:   @property 与 @x.setter
来源：http://hz.nanxinkj.top/gttydfesqv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtfwskzgnt.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtwtjlmtpl.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtmloqoefq.html

Java: public String getName() { return name; }
来源：http://hz.fzhhl.top/gtilccqjxi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pycfn.com/gtsngnypqc.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gttfdcputz.html

C#:   public string Name { get; set; }
来源：http://hz.gotoacloud.top/gthigrudmi.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtupfttdau.html

Py:   def __str__(self): return self.name
来源：http://hz.wangdashe.top/gtdkiisvap.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtlawmljli.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtafeglvst.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtlgbsibcv.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtpltlwnqz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtbruojsog.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtzanapkxx.html

C#:   public override string ToString() => Name;
来源：http://hz.ehwqpu.com/gthvivmidp.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtshguagvb.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtmofxpced.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gttaxlmced.html

JS:   u instanceof User
来源：http://hz.chenlongwang.top/gtrtotodou.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtumlwebfs.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtrtmxphbr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtazemehwt.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtuxrkdztc.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtswygfzll.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gteqgjblff.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtkbayojwd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gtpowljpgd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtyeouzidu.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtbsxuyrhi.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtjwgqtide.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtoswkaijr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtvnlxxhhd.html

C#:   record User(string Name, int Age);
来源：http://hz.hywenlv.cn/gtswfxkwil.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtkpkkmkwx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtckqjnaot.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtjizpruae.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtbvqdmsxw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtvdxvnfzh.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtplodxuol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daxiang520.top/gtdhclyxrq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtwfnnyhpl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtkspiltuq.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtvxhtihzs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtaviaghlj.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtjrujffso.html

JS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtlyjiyyqb.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtnpczqexe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtveinxykc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gtzkhmlfyr.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtosoyoxto.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtfkiggybo.html

================================================================================
来源：http://hz.jianghu66.top/gtuvxgieyr.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtcqtdhmek.html

================================================================================
来源：http://hz.cqqwz.cn/gtrekkgorw.html

[H01] try / catch 基础
来源：http://hz.gogol.net.cn/gtfejhoqkk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gtatrfhkpw.html


<!-- 参考信息 -->