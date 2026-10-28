代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtqdxilxke.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtmjfspykx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hongshengwenyu.top/gthvjowaep.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cashguo.top/gtlzjkbmwf.html

[E22] 字节长度与字符长度
来源：http://hz.wangdashe.top/gtqbqzhkgu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtwjisfnar.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtbejrnefl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtabicrzuv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtcyusbmcc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gtmdhmiwhj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shangyingyoupin.top/gthwskeqrg.html

Ruby: s.bytesize;  s.length
来源：http://hz.tianlin.xyz/gtbhsczwmv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxuanxn.top/gttgqwujes.html

================================================================================
来源：http://hz.ybcxt.top/gtjloffslj.html

F. 文件与目录
来源：http://hz.wangdashe.top/gtfmiabenh.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthzwdaqgq.html

[F01] 读取整个文件
来源：http://hz.ywan-chungtsiang.top/gtaeixfgmo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtvtbwuxwx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtnjlxsisz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xingfuxueyuan.xyz/gthbzvaypk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuanzhike.top/gtlhqllcdk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtymyhxiip.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.snrcjt.cn/gtaudlsqvi.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtygorfzva.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cucudq.cn/gtldfzlruk.html

[F02] 逐行读取文件
来源：http://hz.jianghu66.top/gtuybararx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtqnfivxro.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cheryme.top/gtyuusgwxo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtkhvwuusp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtxrbobxkz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtzubbjaln.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.andypj.xyz/gtdihohuio.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtvpkjooje.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gttbdndacg.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gttnegedbc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tianlin.xyz/gtllxkaovu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtncavymev.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtrzgkfhlf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtxejrrjam.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtsepuesto.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtpgavojvn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtogiqqdix.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtjifjlrjf.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtwlkhtzfs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtwjedjidp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gttyauusxs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtjzkmfnaj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtjshxvsmw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.haohaochexian.top/gtdntfpbbh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gtthxudlkl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gttfokpsko.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gthcodawfm.html

[F05] 判断文件或目录是否存在
来源：http://hz.gzhubu.top/gtudcqzhqv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hfpthk.cn/gtsijppkbv.html

PHP:  file_exists("a.txt");
来源：http://hz.sysykeji.top/gtzqntuqlv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtgvclxvff.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtfslfyvnl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtdgnbuyma.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinyuanbaomall.cn/gtaebcpzzd.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtqtwrtxiz.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtrpbaeqzg.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtbqzzgfug.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258888.top/gteuertnrr.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtrmjqnvkv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtqxwvloij.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtpzdgflfq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtkmywliub.html

Go:   os.Remove("a.txt")
来源：http://hz.ydjk.org.cn/gthnnxvixj.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtsgvbiose.html

C#:   File.Delete("a.txt");
来源：http://hz.havefunace.top/gtphfymytn.html

[F07] 创建目录（含多级）
来源：http://hz.ppjwa.cn/gtpfgncglq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtpijdaune.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtbbzsltjk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtvtanhnvk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtyazbgcns.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtbqublypk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtkshugxpq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gtrobzcfpp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtvajeyksz.html

[F08] 遍历目录
来源：http://hz.guannengcc.top/gtoersunkl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuxming.cn/gtjtabgmkh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gtmkzvufmu.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtvpsrnghh.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtfjmzqiwg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtlsvdkeqo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jlsjyb.cn/gtkdvarnhd.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtvwjbhggf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtvjzksfvr.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gtkomtomqm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtbnvqfffs.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtkecwhnbo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtlpsbqxlv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtitobrzda.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gthkdsqwrd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtjgyfwcnl.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtpitemzwu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtnkdeckoz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtvpeidntu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtxnnmdmmj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuanzx.com/gtillszkcz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtukyjuddz.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gtynjbcxnn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guannengcc.top/gtcsirifjk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtdjmkjvmf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtmbbrhymt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmhgkugle.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gtwensalgx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtnscbsfsr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydjk.org.cn/gtsfcowgrx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtnupbmxbu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtfigruyyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtzjakpsxk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtthcwudpr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtxrmxsqez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gtpbtncljx.html

[F12] CSV 读写
来源：http://hz.ydzc1.top/gtqdcmwzag.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtgvevccon.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtdyieapun.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gthtyvmggg.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtkcwndbxd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtdmbebhru.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtdcutumez.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yangfankeji.com/gtopezxvpm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtpqsmdluu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfzqhvssm.html

G. 面向对象
来源：http://hz.sweek.top/gtazngylwd.html

================================================================================
来源：http://hz.yongpay.top/gtubggrdcj.html

[G01] 定义类
来源：http://hz.aizwys.cn/gtzzsfzdys.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtfhcsdmtm.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtcejzxoop.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtfbxarycx.html

TS:   class User { name: string = ""; }
来源：http://hz.zhoulong.xyz/gtixqzvaox.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtcsrlzxmr.html

Go:   type User struct { Name string }
来源：http://hz.sysykeji.top/gtavfqcixw.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gtremspchk.html

C#:   class User {}
来源：http://hz.wangdashe.top/gtokyawopa.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtpjezoqjy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.kuanghao11.cn/gtuatddgqu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtaagrddhs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtkoitgkwk.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtmwlwzhor.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtbredklvd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenzaomai.com/gtjlwapgtm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtfjoqjjmp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cqqwz.cn/gtamliumzk.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtybfcriun.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gteseftdff.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtybupvpxb.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gttmxzcdzv.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtbdtxfjrg.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtnsdbozmf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gotoacloud.top/gtndeutivy.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtmmqhccnb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtesayocls.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtvvdhdwqt.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gtumhggpkd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtisimmlyd.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gttozzddat.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtkqvtkwhi.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gtjzdlmebe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtdrevpoyy.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtdkpwabuz.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtrhewowyn.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gtznllswvj.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtmvcljfcx.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gtdmyrfnbh.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtonyhrlcm.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtvqaixlvb.html

Java: class Admin extends User {}
来源：http://hz.snrcjt.cn/gtgjvwbpam.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtnbraruet.html

Ruby: class Admin < User; end
来源：http://hz.ivvv.top/gtbdqisnxx.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtkeioimeg.html

[G06] 重写方法
来源：http://hz.shanyushiyangkeji.top/gtkvrjzhxq.html

Py:   def greet(self): return "admin"
来源：http://hz.feifeiyinyue.top/gtlgixbrqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtkkumwkqc.html

JS:   greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtayzyftfb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtirjbsfpk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gteeeunccx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtlslqqwdc.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtrwgbernx.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtleirddmp.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtzvdfiuxf.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtxrmuvzxa.html

PHP:  parent::greet();
来源：http://hz.jyoumei.cn/gtxrtthsmc.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtufsoxems.html

TS:   super.greet();
来源：http://hz.chenzaomai.com/gtwrqiiuqb.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtztmawjbb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtxogprhdn.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gtvaqkaejp.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtxddbpnxb.html

[G08] 静态方法与属性
来源：http://hz.gzhubu.top/gtkxdreeiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtqldhvhrr.html

PHP:  public static function f() {}
来源：http://hz.yueranfly.top/gtrjgidqhf.html

JS:   static f() {}
来源：http://hz.shuidangran.top/gtwtudbqrw.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtggfedcww.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtgdmphfbq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtaqntpjme.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtxnnupfjh.html

C#:   public static void F() {}
来源：http://hz.gzhubu.top/gtvadspsvn.html

[G09] 接口 / 抽象类
来源：http://hz.jiagoushi.top/gtgualtgnq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtjivcybkx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gteyxdhtvz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtnaojmzpe.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gtamdocvgj.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtbknybbmc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gotoacloud.top/gtfdyrifzj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtnhhztpbt.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gtrzziuidh.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtleucnbge.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhengqikj.top/gtttsbcxxe.html

PHP:  public / protected / private
来源：http://hz.havefunace.top/gthmvjidyk.html

JS:   #private 字段；其余公开
来源：http://hz.zhijiandao.cn/gtigqimsfk.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gtbtikksqd.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtsoqgqogi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtezrzizwa.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtlbxsrdsz.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtkdyxovex.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtifimpzxb.html

Py:   @property 与 @x.setter
来源：http://hz.9152youxi.cn/gtzhnbbwpp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtvjlzqvnm.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtowsiczji.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtvwyfqqxj.html

Java: public String getName() { return name; }
来源：http://hz.hnqzz.top/gtufphxhxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtieuvobtt.html

Ruby: attr_accessor :name
来源：http://hz.mhx1999.top/gtbajwkiza.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtqlznqheu.html

[G12] 对象转字符串
来源：http://hz.gaohongyu789.top/gtgyztjyal.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gtplhcrjew.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtzdqdgbrn.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtcbskmblk.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtoqbllrir.html

Java: @Override public String toString() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtufqvqqyo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtwrlpinsr.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gtlxazftcg.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtxuybnunl.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtklcgyxvh.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gtifkxlznn.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtbwijxnmt.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtdsepoqpq.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtlagsxqcs.html

Java: u instanceof User
来源：http://hz.feifeiyinyue.top/gtuchwxero.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtyrfubzfh.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtvcinglrc.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtykroggwr.html

[G14] 数据类 / record
来源：http://hz.hfpthk.cn/gtkdpupgcw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtuxzdhaoh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtabpkfkta.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guannengcc.top/gtbjyeoppu.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gteaymprlb.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtsjthikef.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtubtntmkq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtzqeynfcp.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtlehwnpyg.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtennrczsa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.mhx1999.top/gtfjmvhrwd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtmythhcpx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tianlin.xyz/gtnqamdtur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtokhfjoib.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtrczevgmb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtlbpvphfj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtlmhctnow.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtsteazrph.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtcgghmdbq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtzvokwijx.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtvbxzinoj.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtypegvhro.html

TS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtjxttouab.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtblybkfmv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtuopcrtpi.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtgyunqyxf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gzhubu.top/gtmqukqymc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttxpiogqv.html

H. 异常与错误处理
来源：http://hz.chenjidiqi.icu/gtwqskeudo.html

================================================================================
来源：http://hz.xylfe.cn/gtrzbwwbvz.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtqyxaofgp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtlgochnez.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtklxjjprt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtmkgfliwj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gtzyixskgo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtqvzzwzab.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtubzcinbx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuanzhike.top/gtbgnbcvbx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtypwtfjoz.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gteitgusun.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtvierrzep.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtvsvxhgvk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtqomwlwmm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gthmdegknr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtbygbukpl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenlongwang.top/gtdvctujnc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cashguo.top/gtylrevflj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gtgtwwjlnx.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtnhyluzam.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtesehgoqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtffpmnvgc.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtidviqmvh.html

TS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtaalrxwjv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtyihhtvhv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtvcshetjm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtoyjpqwvg.html


<!-- 参考信息 -->