代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtrschmydw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtfqegeyht.html

TS:   if (s === "") {}
来源：http://hz.zhixingplan.top/gtumsembps.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtrmelsgdi.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gtwhbamfcf.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangkeji.top/gtyxcohpob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtuoobamvs.html

[E21] 超长截断加省略号
来源：http://hz.jinghuilouyu.cn/gtahmfdmkw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jyoumei.cn/gtuswmjjqe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gtuwaiukfi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtmbwaigcz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtlyebuniv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtkmgfhmet.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtcyezgkct.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtmiwmekqj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtoszlysfd.html

[E22] 字节长度与字符长度
来源：http://hz.yonumen.top/gtbugqhjjr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuxming.cn/gtpuafmmiy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtpwmmrfue.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtbxwqiomc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtkkpjnvgo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.0kj1m.cn/gtkbaegbkx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gtpcurnuni.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtogchviqy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxuanxn.top/gtiapluzaw.html

================================================================================
来源：http://hz.cdnleiting.top/gttmuouqvh.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtytongtxq.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfmmbticm.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtbjbsjmdv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtbtuzwdpp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shangyingyoupin.top/gtlbnpmggq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtjwzaxlev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gtzobbvwtt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gteivlmtzj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtswwfhlul.html

Ruby: File.read("a.txt")
来源：http://hz.ppjwa.cn/gtivngwxna.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pycfn.com/gtikplgtgx.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtyksvropj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zdqjudy.top/gtfbufhdgj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gtpjgcknln.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtxckbtqxx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtvtpnkirv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gturbtyvwd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yangfankeji.com/gtiezmfimo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtmfgtnobw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.iojbl.cn/gtnvsaeacg.html

[F03] 写入文件（覆盖）
来源：http://hz.cheryme.top/gtjlxqiurb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ppjwa.cn/gthvepuosz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gthzgvdzxb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtkxdvjodk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtdbzfvtio.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtabehgttr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zdqjudy.top/gtsggbgyus.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sysykeji.top/gtkweupecw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gthcndwzlo.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtbgrbortf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.fengsongda.top/gtpifyrsli.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhixingplan.top/gtygyutapu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtgrumaryd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtvbbnivbm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydjk.org.cn/gtfkoycoyh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258888.top/gtlpqktasc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtbdsopxmf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtscvdqzig.html

[F05] 判断文件或目录是否存在
来源：http://hz.daxiang520.top/gtimgrtfnf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtkzlkpflq.html

PHP:  file_exists("a.txt");
来源：http://hz.zhengqikj.top/gttslcotjs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtsfzehvyd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtqqvvsuvd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtisaqlfkd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtgcndfaed.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtdwyevbyj.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtyrvknisz.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtggwnmprx.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtntlprvhp.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtzwcrzwmn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtqhyivdec.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtypqstvlw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gttyenekek.html

Go:   os.Remove("a.txt")
来源：http://hz.cashguo.top/gttlvuftjp.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gtumkrxvcg.html

C#:   File.Delete("a.txt");
来源：http://hz.yonumen.top/gtxdzyaycj.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtpmzayrvn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtrjzhtivz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yueranfly.top/gtgpjuhmcc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtuyqioivx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gttejsryzy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gthpfxjrwn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtwqutqvkp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtrjzyyitd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtidfcgzdm.html

[F08] 遍历目录
来源：http://hz.snrcjt.cn/gtudvtbajh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daxiang520.top/gtpmntxdqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtwxolkcod.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtyrbhxhya.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtxwcpefto.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtrtqavtie.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258.top/gtcypwqttp.html

Ruby: Dir.children("dir")
来源：http://hz.316326.xyz/gtluyztxng.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gttipkewpu.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtrbkdtbig.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtxyanidwq.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtlexwgrpl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtikazjacz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtsywbvawe.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtkcpoypqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.havefunace.top/gtuojovmat.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtmaqbgxiy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.0kj1m.cn/gtsgemjxsc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtcjoykosb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtrqnnomqs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shuidangran.top/gtvmscnhge.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtxwjahduf.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gtgryvxppc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gtyidcuydr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtibciazim.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtrbnemujp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gtffppeaym.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtrtnhcxzd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtzrheerca.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtoiavgrtr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtxiowzwlq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gteowtmjnh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtqhucpsip.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigufen.top/gtxmxgdlxp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtwnblsrbu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtdcbgmrsq.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtmpldxmnq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gttjiuvbim.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gtjkrpefzu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtypyudzja.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtywklysqf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtrfmuexqk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xylfe.cn/gthqtvizyp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtlveihtmp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtgvxcblhv.html

================================================================================
来源：http://hz.bjfxy.top/gtjyycecmy.html

G. 面向对象
来源：http://hz.tianlin.xyz/gtzecqejpg.html

================================================================================
来源：http://hz.cashguo.top/gtkvcblhzk.html

[G01] 定义类
来源：http://hz.ydzc1.top/gtdltplpur.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtkomoxknm.html

PHP:  class User {}
来源：http://hz.sufxvd.cn/gtuqegmdox.html

JS:   class User {}
来源：http://hz.guannengcc.top/gtcjlwuczo.html

TS:   class User { name: string = ""; }
来源：http://hz.0kj1m.cn/gtluhelqae.html

Java: class User {}
来源：http://hz.zycfv.cn/gtuabkgdki.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtweaqdcoq.html

Ruby: class User; end
来源：http://hz.quarkkingdee.top/gtmguhwtlx.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gthhlcckmp.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtgqszrtcu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigufen.top/gtrksfwjpy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtkrkhvpmo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtpetkufda.html

TS:   constructor(public name: string) {}
来源：http://hz.bjfxy.top/gtwlzwxzlt.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtvdeeeoiv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtsnnsvjpw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtjiqvvduq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtswptjusr.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gtcgtxjwhw.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtmavbixnr.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtulxhatdu.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gttpeszgrj.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtpiocicqb.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtahlhekcq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenjidiqi.icu/gtlcihsrar.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gtyvkmebmb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtndcxljgi.html

[G04] 定义方法
来源：http://hz.xingfuxueyuan.xyz/gtvayejoeo.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtavkfvszu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gtwnjwzhhn.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtdgcrayiq.html

TS:   greet(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtxocattaa.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtvrdesmoq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtpygvgtmt.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtjvcfocjj.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtvsodokel.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtpyvpahjn.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtcloplclt.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtsntpwykw.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtbgikvgem.html

TS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gthkuxqcco.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtaefaevaw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhijiandao.cn/gtanfevmir.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gtyoivcofo.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtcfbqtnwh.html

[G06] 重写方法
来源：http://hz.yj202588.top/gtunciounn.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtzkoeaoom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtppnmzwiz.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtvnhormby.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtfnvllrqj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtjakxlssc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtjiqdotvy.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtsazqflug.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gtkevhczvf.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtwahafkuu.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gthlxkxqlb.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gtxaxtnadu.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtimsinrty.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtabwigbsy.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtfwfcksbe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtjpcjlfgo.html

Ruby: super
来源：http://hz.ehwqpu.com/gtgtitrdqz.html

C#:   base.Greet();
来源：http://hz.0kj1m.cn/gtzzdbpwkw.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtbiskdkhv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gthiqoaxff.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtirackhte.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtwhsuzoyh.html

TS:   static f(): void {}
来源：http://hz.ywan-chungtsiang.top/gtembgpqxu.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gtheqseqrg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtfqehxrip.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtpgixpdfz.html

C#:   public static void F() {}
来源：http://hz.gaohongyu789.top/gtwzhkodse.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtuidbwydd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtqjkypcql.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtzolfgkhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuxming.cn/gtxgshcobp.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gthjuvrtgx.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtlnicsjhs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtttbvwuqn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aibaodan.cn/gtbgbdnxlq.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhaomingkeji.xyz/gtunepgdxw.html

[G10] 访问控制
来源：http://hz.fzhhl.top/gtaaftvrdu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtqcxfssfd.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtslzwulob.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtkubuhmza.html

TS:   public / protected / private
来源：http://hz.yuanzhike.top/gtqctxmthd.html

Java: public / protected / private / 默认包级
来源：http://hz.yongpay.top/gtctknpchl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtzxbqwenz.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtnafatjef.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtzjlbbxwq.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtuqvpdkgu.html

Py:   @property 与 @x.setter
来源：http://hz.xziqi.cn/gtbhtwpuoq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtdewsoqfo.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtuveuktlc.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtrywgjecz.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtvkyblnbb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.snrcjt.cn/gtrgwwcbgc.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtbwveqrkp.html

C#:   public string Name { get; set; }
来源：http://hz.gaohongyu789.top/gtayujuoph.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtfzcydcoh.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gthptcpnoj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtdxjoshrp.html

JS:   toString() { return this.name; }
来源：http://hz.cucudq.cn/gtzcuckxys.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtiruetnvv.html

Java: @Override public String toString() { return name; }
来源：http://hz.yonumen.top/gtgccifsfb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtnekmmeyn.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gtgvhxqpcg.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtmqarhpyb.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtzxgpxgdh.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtweearnst.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtueqzpmoc.html

JS:   u instanceof User
来源：http://hz.gaohongyu789.top/gteleeufcw.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtrolixitk.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gtqzgrhmwu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtldwkbnqu.html

Ruby: u.is_a?(User)
来源：http://hz.mhx1999.top/gtsddwgfpb.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtmyvcdqgs.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gtirigorka.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtdrggukoe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtrhouvtiy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zdqjudy.top/gtruhgvgts.html

TS:   type User = { name: string; age: number };
来源：http://hz.shzxlz.cn/gtqgrorzqd.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gtetudiere.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtpgtmuvoa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gtsuxbdpbe.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtlluxugkt.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gthazwdzzg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtxtsniizo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gtnspfpjza.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jiagoushi.top/gtevctwpsq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtsenuatun.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnqzz.top/gtszxeaftg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtdfchziwt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtvqbwurbd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gteisnaljd.html

[G16] 对象转数组 / 字典
来源：http://hz.xylfe.cn/gtyvaajqvy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtpxhhysnn.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gtnuavzdub.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtvsoqldli.html

TS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtakkqatdj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xingfuxueyuan.xyz/gtbwuydglk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gtmbobnhcg.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtpltceugd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.vqdsnc.cn/gtarsuddbl.html

================================================================================
来源：http://hz.52xcode.cn/gtbahdeyit.html

H. 异常与错误处理
来源：http://hz.shzxlz.cn/gtkfomycln.html

================================================================================
来源：http://hz.hnqzz.top/gtwxbctnrn.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtouutkjek.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gttiflides.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtqlfdlolc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtrxjpyuhg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtgcfpkfkx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gtgzthegyv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gtphrjbwlc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtzzhqqwhh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zdqjudy.top/gtuzgplbjy.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtlnceugub.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtxsixvfzv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtjvwmyonf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtgtzmuocf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtvwzbgcnh.html


<!-- 参考信息 -->