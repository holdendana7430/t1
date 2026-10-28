代发 wailian999

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtinseqrcv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtnrojlzlb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtabzussfb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtcxdeictd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtrtxmyvyg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtmzvvygfx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gtjscefwzb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnqzz.top/gtwiexuhxr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtyrpaaqpi.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtqnpxvpcp.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtpqqrylpm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtuzgpgwdy.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtekdpqrvp.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtufjqzmyf.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtpgqtwdrf.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtrtkzxgjy.html

Ruby: s.lines
来源：http://hz.bjfxy.top/gtwdvedoly.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtrydfaehu.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtehgafahs.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gticpwcnci.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhaomingkeji.xyz/gttjrplyxz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gtdagjtakr.html

TS:   if (s === "") {}
来源：http://hz.mhx1999.top/gtlfgresdz.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangdashe.top/gtuvsdnykh.html

Go:   if s == "" {}
来源：http://hz.daria6918.cn/gtmcrwdszg.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtcgcwtpqk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gogol.net.cn/gttijfxohj.html

[E21] 超长截断加省略号
来源：http://hz.shangyingyoupin.top/gterfutunb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtnrbcwxhp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.feifeiyinyue.top/gtxkfjusbs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtpzucjufo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtozyfmpzz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtddjsqnut.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtfozbqygk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtptlvngrg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gttdrdozaf.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtwlxeehyp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtjpaougju.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtiyxucdhy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xinyue.icu/gthurficvq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtpjljvabp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hongshengwenyu.top/gtwgolumtj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhoulong.xyz/gtgylgapgc.html

Ruby: s.bytesize;  s.length
来源：http://hz.gogol.net.cn/gttjlydqem.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hongshengwenyu.top/gtezpuxgal.html

================================================================================
来源：http://hz.gzhubu.top/gtsinjixiu.html

F. 文件与目录
来源：http://hz.dashuyun.cn/gtrunvamyo.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvfhmuxct.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtqkwvkpje.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtdctsnuxt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtfbmvkmkt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtmnonssee.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtnnznnuum.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtrnneayfm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yonumen.top/gtdeylzsrk.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258888.top/gtaucuvwei.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtcvwpifov.html

[F02] 逐行读取文件
来源：http://hz.andypj.xyz/gtrechzawx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ivvv.top/gtpkbyhija.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.feifeiyinyue.top/gtblerftel.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtxtpncbrt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtkguepkgp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtbfjiqagh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtrmhfrihh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jyoumei.cn/gtustcmaxq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtcwkehqyz.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gteistgsqz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nwbrower.top/gtfzzbgdld.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gteeuczmiz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtuxkozpiq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtjeaugkmh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yonumen.top/gtasqdatry.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtahkluhjh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhongyouzk.top/gtjalyhmpy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.c1oappe.top/gtknopxiai.html

[F04] 追加写入文件
来源：http://hz.cqqwz.cn/gtjusilquj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnxiangtu.top/gthswtjbji.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuanzhike.top/gtytdlnapr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtujjfvdyl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtjgobauzh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guowangkeji.top/gtqlwsxdfl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shzxlz.cn/gtducfblyj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gtbrowwgac.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhengqikj.top/gtqpzyresz.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtueodynsk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ywan-chungtsiang.top/gtqxzugacy.html

PHP:  file_exists("a.txt");
来源：http://hz.cheryme.top/gtduktyyzx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtntpjxyij.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtrmtujrgp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtzryqsuij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtsydmaqgz.html

Ruby: File.exist?("a.txt")
来源：http://hz.dianchejie.cn/gtghxxcxjz.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtbptrdiba.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtckmfcxlc.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtvekllcsi.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtzngejczh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtufulgcxd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtuliduksf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtllqdkpem.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtuwnyyedz.html

Ruby: File.delete("a.txt")
来源：http://hz.hnxiangtu.top/gtqzdnfbgo.html

C#:   File.Delete("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtmdzoziir.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtpsrgpfkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydzc1.top/gtvxbgvamq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtqgkdefdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtuzuvwgma.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtruonykhw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangtech.top/gtkzcaxlcf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.birdmap.top/gtyfihabms.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ivvv.top/gtetuhfrhc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj202588.top/gtykqenprc.html

[F08] 遍历目录
来源：http://hz.jinyuanbaomall.cn/gtcplwgydm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.feifeiyinyue.top/gtbevtxfpf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtcwwvykff.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgufenzy.top/gtryeplbip.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gthbbuzina.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gthzxzvkol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shuidangran.top/gthofoogwl.html

Ruby: Dir.children("dir")
来源：http://hz.xinyue.icu/gtwhogyywd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.snrcjt.cn/gtzhveyvmj.html

[F09] 获取文件大小
来源：http://hz.shzxlz.cn/gtoskczkwr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtsjoozxgp.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtnlxvwuck.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtzhjumgek.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtrubpajmp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtflvcgblm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.redwolf501.top/gtpiwwgght.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtqqlsmvtw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtvbqtjeqp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtlbkfbxed.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtyozqnoow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtxpexvufd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtxzzvsnyt.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtgefonbvv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.iojbl.cn/gtywaqqgil.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.iojbl.cn/gtphdgvksw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtxpixoiem.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gtroazxldw.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtfhnwloiw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtxxqfdemc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtvykalija.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtzbkzgxzl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtjnidhvel.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtypxphnnf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtmvmnvsbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtkzjtbmym.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gtxzioztrf.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtykzqdesi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtqtzodjqz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shzxlz.cn/gtuicpsweo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dianchejie.cn/gtanmososr.html

TS:   // 同上
来源：http://hz.jiagoushi.top/gtooltlmvu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gaohongyu789.top/gtmvqvjylx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhijiandao.cn/gtejgnyfdc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtkyssxcym.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtlvtihugh.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdrmyzfgq.html

G. 面向对象
来源：http://hz.tanke756.top/gtnjavmwgv.html

================================================================================
来源：http://hz.iojbl.cn/gtggcvugzt.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtkfpelcxx.html

Py:   class User: pass
来源：http://hz.ivvv.top/gtldgvwidn.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtasdasjvt.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtrtbjugbw.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtmsbfjcxj.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtltwriyom.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtfjulzsqz.html

Ruby: class User; end
来源：http://hz.gzhubu.top/gtzoxxzune.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtozpoliyi.html

[G02] 构造函数
来源：http://hz.gzhubu.top/gtzypltmgn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.bjfxy.top/gtkddhursh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gtxhytihga.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtbblufnzf.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtlzybycbp.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtfnurzbmd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtenizthwx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gturybpdts.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ehwqpu.com/gtocwzlzhf.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtwxxsotuw.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtpfwufqxr.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtnettoijg.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gttfbcazvb.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtudzckfjz.html

Java: private String name;
来源：http://hz.yj202588.top/gtezhofecr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtjnapioem.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gttzuwmwxj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtfytgmowr.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gttfdhkfvq.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gthdjxzcrl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtbgodpmsg.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtcmnqctzv.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtehmxegnm.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gthhqvwwqj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtsuvulcbg.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtqyligxxa.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtwztotoji.html

[G05] 继承
来源：http://hz.yuxming.cn/gtlpyvgctk.html

Py:   class Admin(User): pass
来源：http://hz.ehwqpu.com/gtubtzytyc.html

PHP:  class Admin extends User {}
来源：http://hz.nanxinkj.top/gtjuipiqrr.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtrefulrcr.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtesnyxcng.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtxfsfzzlt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtqnfbfizj.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtrdwnivsu.html

C#:   class Admin : User {}
来源：http://hz.kuanghao11.cn/gtwvktlsku.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gtfeewesio.html

Py:   def greet(self): return "admin"
来源：http://hz.yangfankeji.com/gtdmzimvjw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtdbrhktjj.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtsjxnrwka.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtdfotrnps.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtwjkocdsn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtxhmasckt.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtbeadnntf.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtfewjrqgo.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gtutjztzik.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gtxezoylxa.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gttxrnqtds.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gttcwuzqsu.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gtpofvmnlc.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtzmmnnlds.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtwucyuaer.html

Ruby: super
来源：http://hz.zhaomingkeji.xyz/gtmvimpdyn.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtrlkznrdx.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtlarkjvwb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtnhrajype.html

PHP:  public static function f() {}
来源：http://hz.yvedp.cn/gtgylpinxa.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gttwjrxeba.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtokinstbl.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtbolticjs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gttbjvwwhp.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtoovbrste.html

C#:   public static void F() {}
来源：http://hz.aizwys.cn/gtazdhsaiq.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtcrjszwjw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtvpiwtphl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gthxyzkavm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtnawphydv.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtnsntoscr.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtyslabcjw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gtcqtllezz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtpkuqjzwv.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtzmbtjqqs.html

[G10] 访问控制
来源：http://hz.tanke756.top/gtoyudqgsu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtywvpksmi.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtmiomkfco.html

JS:   #private 字段；其余公开
来源：http://hz.jinghuilouyu.cn/gtvifmrvzk.html

TS:   public / protected / private
来源：http://hz.redwolf501.top/gthrraggun.html

Java: public / protected / private / 默认包级
来源：http://hz.zhixingplan.top/gtsonxslan.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtpplkrvzt.html

Ruby: public / protected / private
来源：http://hz.zhoulong.xyz/gteaycknhc.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gtwaknudmw.html

[G11] getter / setter
来源：http://hz.zhixingplan.top/gttdmiiexs.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtogjkbhro.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtyocezryv.html

JS:   get name() { return this._name; }
来源：http://hz.ydjk.org.cn/gtmakujxgw.html

TS:   get name(): string { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtucctiyqd.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtvwftuvcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtjstlnjqo.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtmahrdjig.html

C#:   public string Name { get; set; }
来源：http://hz.hnxiangtu.top/gtpvmmnnbl.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gtykucokmn.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gtwfxhhoep.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtwpbitgiv.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtingnunex.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gthjobjmhz.html

Java: @Override public String toString() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtdybpjygx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgfzy.top/gtdwtazmxs.html

Ruby: def to_s; @name; end
来源：http://hz.jlsjyb.cn/gtenrtdsna.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtlpiydoct.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtjamxzpjd.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gtwqwgqkyc.html

PHP:  $u instanceof User
来源：http://hz.xuanzx.com/gtaquuntlx.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gtfmyhekhr.html

TS:   u instanceof User
来源：http://hz.yueranfly.top/gtxkeiquhu.html

Java: u instanceof User
来源：http://hz.guannengcc.top/gtuhpgsapr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.mhx1999.top/gtenyltpcc.html

Ruby: u.is_a?(User)
来源：http://hz.zhiwuduotai.top/gtteivlrtw.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gtbombdljj.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gtiyroydxj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gthrmjxxet.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258.top/gtpcjzgjtx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtuspsdduh.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtbjaulecq.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtypzvorip.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtngfexbqr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtupmzkgnb.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtvsgtiork.html

[G15] 枚举
来源：http://hz.birdmap.top/gtvqbbylhi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtlhitafvv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtbmgufxnb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yonumen.top/gtidiizexh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtoceorhqh.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gtiwbykdyv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtxdbdakjo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jlsjyb.cn/gtlauaojyn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtfrdhrjhu.html

[G16] 对象转数组 / 字典
来源：http://hz.hnqzz.top/gtctmyivxv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gtiymztnia.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtmdueynlm.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtraghkjmo.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gttmiasfky.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtenlanizy.html


<!-- 参考信息 -->