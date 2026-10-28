代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.andypj.xyz/gtkujvykim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtojdrhjmf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtpxshwktu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hfpthk.cn/gtdfgsehtc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtcaechfgn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.quarkkingdee.top/gtadkpztib.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtqxoaztdk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gzhubu.top/gtpsnsklzc.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gttwaiwgnv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xziqi.cn/gtiubxvocq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pengpengdd.cyou/gtysbpudaj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtlewwsybu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtcghakhbx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtvpfyfhng.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gthzwtqsdu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258.top/gthvkjyehm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hywenlv.cn/gthbdztefq.html

[E19] 多行文本按行拆分
来源：http://hz.cashguo.top/gtxpxnhzfz.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtqaidkkve.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tian-w.cn/gtfkgahjie.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtujodranl.html

TS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtpqanwjba.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtmerfnngz.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gthxmywvcy.html

Ruby: s.lines
来源：http://hz.yj20258888.top/gtzgdeezdx.html

C#:   s.Split('\n')
来源：http://hz.ybcxt.top/gtlxhmzgig.html

[E20] 判断字符串是否为空
来源：http://hz.nwbrower.top/gtkushudri.html

Py:   if not s:
来源：http://hz.hammf.cn/gtqbvnloof.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtmunlaych.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.redwolf501.top/gtwoamtzva.html

TS:   if (s === "") {}
来源：http://hz.feifeiyinyue.top/gtywsciwwm.html

Java: if (s.isEmpty()) {}
来源：http://hz.xziqi.cn/gtaojpjpfl.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtzetokyvf.html

Ruby: if s.empty?
来源：http://hz.sweek.top/gtupmxitfh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gtuajnlomi.html

[E21] 超长截断加省略号
来源：http://hz.wangshuangyany.cn/gtcebogttu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtgvdzmact.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xuetiantiany.cn/gtrjkyekcj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtgsetaklv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtenevgumz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtommufpli.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gtdcozwdfo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.svipenyu.cn/gtimhduout.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtfkcuhmoz.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtlbxikvzg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.316326.xyz/gtkmoyeawo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtgvqhfyuz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtbaxvjojh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhongyouzk.top/gtczlklafa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtvwqncawa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.mhx1999.top/gtiafrdxll.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtlreycbrh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangtech.top/gtuqitsdwe.html

================================================================================
来源：http://hz.hfpthk.cn/gtrrdbdrce.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtjbrlcyfs.html

================================================================================
来源：http://hz.zycfv.cn/gtqjxsxswz.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtatqjbrjq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtcvkjjtqf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtoqlrafof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtyvkumgra.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.svipenyu.cn/gtazbnxmtv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gticnbsrzv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtxluyjdoy.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtdfbwxwxr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtfpreocuy.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtqmydfzrg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sysykeji.top/gtueqfrvhz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinghuilouyu.cn/gthqdaaqbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtbtdofpur.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtsmlfdorm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtdghuypwd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gtobznbhon.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtdpvjnrmb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gtywoxyjhr.html

[F03] 写入文件（覆盖）
来源：http://hz.chenjidiqi.icu/gtmrumxcpr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tianlin.xyz/gtlaktuupl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtawnfnzqh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtvxearvyu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtpjwivjvd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.9152youxi.cn/gtoifvltcz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinyuanbaomall.cn/gtaawafbsx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258888.top/gtvstdrgvw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtqwnrjfbp.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtblqqifxs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258.top/gtippkfqjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtpaetsunp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtymbmzmka.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hysaishi.cn/gtngzqnmne.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtqvwgvoga.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtxygjfnun.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtpskuybvs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtprcoumuf.html

[F05] 判断文件或目录是否存在
来源：http://hz.yueranfly.top/gtjssdduby.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtjrprlxqp.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtoewaxezs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtcojchfal.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtinquhcgj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtcoxaztrs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigfzy.top/gtacotxjag.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhijiandao.cn/gtzpiyuops.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtsukhluwg.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtvfpbhhax.html

Py:   os.remove("a.txt")
来源：http://hz.yvedp.cn/gtafyerlmv.html

PHP:  unlink("a.txt");
来源：http://hz.nwbrower.top/gtymzpdroi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gthkjhbuad.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtjknaojlk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtcinnuvpp.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gttoqmcrxb.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtbqdrvgrc.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtqluzimkz.html

[F07] 创建目录（含多级）
来源：http://hz.yueranfly.top/gtfmopvmxk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gthqfdcsfu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guannengcc.top/gtahttavkr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtaeyerwpf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtoohhqcjb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtqfbukorb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gthnwhhblx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtxikhorbd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gogol.net.cn/gtigwatvrd.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtrthyvzku.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtjphjxety.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hammf.cn/gtwjxumwnv.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtjsaunrab.html

TS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtodkzjqbs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtzvxcoprl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hfpthk.cn/gtnvdbgyln.html

Ruby: Dir.children("dir")
来源：http://hz.xziqi.cn/gtxvvrcene.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydjk.org.cn/gtqzdvyqqm.html

[F09] 获取文件大小
来源：http://hz.hnxiangtu.top/gtyhyinmbi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtnghhncul.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gtmvfsmqfi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtyjocbyui.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtyugsrjny.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtasexfmhj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtzaskswsf.html

Ruby: File.size("a.txt")
来源：http://hz.sxryk.cn/gtdwwbxyci.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.feifeiyinyue.top/gtbqpzwlja.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtcaywwnbi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtqoimmbcy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.0kj1m.cn/gtdmcbvvlo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtiidouhga.html

TS:   path.extname("a.txt")
来源：http://hz.pycfn.com/gtsfsmidij.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtoattdbcl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hammf.cn/gtlangdljd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gthcgruten.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtlloehuac.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtzjovqfgy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtjnhhsiab.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtmlyxaxgk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtsrsnisxr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtejmrjwzq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shzxlz.cn/gtwheanqlq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtoqbnhkwe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtsbpnjvtv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gtdmrwbasq.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gtbtwwxhvu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtozoacdxn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtfdfhtztq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtwxkdpujo.html

TS:   // 同上
来源：http://hz.feifeiyinyue.top/gthjieasea.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtisqpsrvs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtaseztogh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gtumbmbanf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cashguo.top/gtwguhrsfm.html

================================================================================
来源：http://hz.cdnleiting.top/gtxhugpxld.html

G. 面向对象
来源：http://hz.ivvv.top/gtnbeilybb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtdjjmdxbo.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtgwriuwvz.html

Py:   class User: pass
来源：http://hz.zhongyouzk.top/gtdtblzflq.html

PHP:  class User {}
来源：http://hz.zhijiandao.cn/gtzatwheuz.html

JS:   class User {}
来源：http://hz.hammf.cn/gthbzalxkr.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtfblildaw.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtzbuwybad.html

Go:   type User struct { Name string }
来源：http://hz.chenjidiqi.icu/gtufezxgvz.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtgpimpsvn.html

C#:   class User {}
来源：http://hz.ivvv.top/gtodtvytbo.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gteqgivxib.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtzmiwbgjk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.havefunace.top/gtkkttkihq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj202588.top/gtwvojoacm.html

TS:   constructor(public name: string) {}
来源：http://hz.316326.xyz/gtwjuoiqig.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtutrikpgv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtzfslsvvs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinyuanbaomall.cn/gtourgmxqs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtyswpxyqz.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtxwyahzsd.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtxddgehzu.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtswqwckzq.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtmeozjasz.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtpihungov.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gtcnishmbu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jlsjyb.cn/gtnbnshnxf.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtfdrefsqb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtcqirphpu.html

[G04] 定义方法
来源：http://hz.hysaishi.cn/gtikmjreqd.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtjkftywvy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtlhhtudim.html

JS:   greet() { return this.name; }
来源：http://hz.sysykeji.top/gtgmemsjdo.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtmhztzain.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtwqozvhnj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtoomfeyzp.html

Ruby: def greet; @name; end
来源：http://hz.cucudq.cn/gtrvefbemy.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtuwznlayo.html

[G05] 继承
来源：http://hz.yj20258888.top/gtofefkfqv.html

Py:   class Admin(User): pass
来源：http://hz.yj20258888.top/gtlfycjgrl.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtjmifeewk.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtczocylbr.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtmmioghhn.html

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gtpkoyxrbj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtaaadacmr.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtkwlnmnbr.html

C#:   class Admin : User {}
来源：http://hz.yuanzhike.top/gtievlauli.html

[G06] 重写方法
来源：http://hz.dashuyun.cn/gtvgjwhivl.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtxxwkyojd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtzuwtxvhf.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtcumghvfx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gttvjpujmc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gthxlsodzs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtzhttylrz.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gtvegjgsdm.html

C#:   public override string Greet() => "admin";
来源：http://hz.yanxiufei.cn/gtfthqaxqu.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtsksyekpq.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtoxtlpqzr.html

PHP:  parent::greet();
来源：http://hz.yuxming.cn/gtbdhyhsan.html

JS:   super.greet();
来源：http://hz.zdqjudy.top/gtqoelhwog.html

TS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtylnidcmc.html

Java: super.greet();
来源：http://hz.sweek.top/gtbetzujla.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtayxdihed.html

Ruby: super
来源：http://hz.yonumen.top/gtmmvyewxd.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtpknvnmhy.html

[G08] 静态方法与属性
来源：http://hz.birdmap.top/gtjqnkjgft.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhijiandao.cn/gtvanapfry.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gthjawqmmf.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtbwpnfwtl.html

TS:   static f(): void {}
来源：http://hz.yuxming.cn/gtshxbkbym.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtxuutblla.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtwcyapzuf.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtxkilklox.html

C#:   public static void F() {}
来源：http://hz.gzhubu.top/gtvoatyzuu.html

[G09] 接口 / 抽象类
来源：http://hz.jlsjyb.cn/gtrzwxzlzr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtholuwglr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtboobqyqg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtaciovsbj.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtiunuzgat.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gthfudwweb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gteguepzhi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydjk.org.cn/gtpogxuxxb.html

C#:   interface IShape { double Area(); }
来源：http://hz.feifeiyinyue.top/gtmncfnowi.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtfhblbjfl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.316326.xyz/gtrcxocsgg.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtoodphcav.html

JS:   #private 字段；其余公开
来源：http://hz.hongshengwenyu.top/gtyssfqbqj.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtuozbpiqh.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gtxdgsxkjf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtxaeiireb.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gtwfyerthn.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtfvuoilsg.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtncvxzipz.html

Py:   @property 与 @x.setter
来源：http://hz.zhaomingkeji.xyz/gtmhomqcgd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtjuctnbho.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtohuqwshd.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtvijjfaqf.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtpmwfbotm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj202588.top/gtklzreude.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtzcetslai.html

C#:   public string Name { get; set; }
来源：http://hz.yvedp.cn/gtxffrzmoi.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtgjhuzyjo.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtbpxbqlqs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtnyomtryh.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtcyxmglvl.html

TS:   toString(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtdzlrqyso.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtkqmzhmxz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.smart0.xyz/gtupwazime.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gtzvbmppje.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtvamemuhh.html

[G13] 判断对象类型
来源：http://hz.nanxinkj.top/gtffsqfapz.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtmtlczwqu.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gtpmnvsufd.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtulhrcaqq.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gthgrrxbne.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtdzumclhu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gaohongyu789.top/gtxuoztihc.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gtptwywxzu.html

C#:   u is User
来源：http://hz.hammf.cn/gtxdykbctj.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gteapsjiyt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtudimpkrz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtmyvhqzdv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tanke756.top/gtsetwkhmr.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenlongwang.top/gtmdiclgag.html

Java: record User(String name, int age) {}
来源：http://hz.c1oappe.top/gtordqoocp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangkeji.top/gtibxlzioi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gttxyhmhsu.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gthzcsgloi.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtujdhtgbm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtzmohomhz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gttvccqzhb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hammf.cn/gtshtylsqc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtbzivalpj.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gthmiqclxb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtzamgycfd.html


<!-- 参考信息 -->