代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.sxryk.cn/gthfsuzzga.html

TS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtdhdaclhc.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtearlrclo.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtezkurlof.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtwbginjcw.html

C#:   s.Split('\n')
来源：http://hz.aizwys.cn/gtazskpmfa.html

[E20] 判断字符串是否为空
来源：http://hz.gogol.net.cn/gtqkcvckyk.html

Py:   if not s:
来源：http://hz.snrcjt.cn/gtmuzhwuea.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtkoqmjvro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtdfosvwjs.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtrcckpkio.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtqkfksctz.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtszlfkohx.html

Ruby: if s.empty?
来源：http://hz.xylfe.cn/gtygixkvqu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nwbrower.top/gtpoyavnup.html

[E21] 超长截断加省略号
来源：http://hz.meibo888.top/gtcrlqhnle.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtvtolgkvu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jianghu66.top/gtrqwetcvv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtkbxhhucl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gteijtnwts.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtsozodibc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtxbihoavd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtddjsozmz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtzttyyiei.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigfzy.top/gtrlqeegim.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.bjfxy.top/gttwnbalpq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtfmwxznoa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gteqwzdufe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtsthmspru.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtgiegvggp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cucudq.cn/gtvsjgtkvh.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtdcdrohxd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtgfannzue.html

================================================================================
来源：http://hz.gotoacloud.top/gtdhqhmsut.html

F. 文件与目录
来源：http://hz.zhaomingkeji.xyz/gtslpgsezi.html

================================================================================
来源：http://hz.sufxvd.cn/gtbjklfezs.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtrbwrntis.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.9152youxi.cn/gtjpdhreyi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtehbfxfaj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydjk.org.cn/gtumyoqozs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtxmmquphi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtauxipure.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gtzuczvley.html

Ruby: File.read("a.txt")
来源：http://hz.cdnleiting.top/gtbcytihye.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ybcxt.top/gtgpurgnrl.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtegdkfypm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydzc1.top/gthvkqcpku.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtinzluxch.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.kuanghao11.cn/gtdvssqtjt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtnvvkhyrt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtghhsxygs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gtucrisitu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jiagoushi.top/gthubigbay.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aizwys.cn/gtyxzewpwa.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtuoxrvwdg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtviommckl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yueranfly.top/gtelkivodc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtjxovtnjl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtzlvbybdo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtvdsarcfl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtdvhqxgvd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtzzmcffrd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtdfvvnrkf.html

[F04] 追加写入文件
来源：http://hz.gogol.net.cn/gteqlewxpk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gotoacloud.top/gtvdvfdyah.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pengpengdd.cyou/gteqohbhnj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtestbaqgd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtruauwoqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtckmwdacf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.quarkkingdee.top/gtgbnqbnqk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hongshengwenyu.top/gtfyctivmh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258.top/gtkpjxhdph.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtpmltqhsq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtqknwqdvc.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtvagxhrce.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtwmvdrbtv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtidokfmbq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtnwvmtdny.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtcssgfuqm.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtrrvywcjt.html

C#:   File.Exists("a.txt")
来源：http://hz.xinyue.icu/gthfukttsb.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtyimppxrv.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtabpzttkn.html

PHP:  unlink("a.txt");
来源：http://hz.xuanzx.com/gtdhmdyksp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtngvnqilj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtxpzmbokj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gttjyqpvwt.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gtccodkybj.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtwnjoezsh.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gthekjlojr.html

[F07] 创建目录（含多级）
来源：http://hz.yueranfly.top/gtfichzqfv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gthmilpoko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtznpbcxnu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtjsktdpsi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtydkqaqlp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtxrptahiq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.meibo888.top/gtgjigpcms.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangkeji.top/gtobvlyrfu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cqqwz.cn/gtuwkoupfo.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gtyhjscfbs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtoavuwgki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuxming.cn/gtfkrzctzr.html

JS:   fs.readdirSync("dir")
来源：http://hz.daxiang520.top/gtimfgakhq.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtxrdsapez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtspabkoie.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ybcxt.top/gtdnxxirew.html

Ruby: Dir.children("dir")
来源：http://hz.iojbl.cn/gtexvpernx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.birdmap.top/gtfaouigsc.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtntjmvasf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj202588.top/gtgwclaumg.html

PHP:  filesize("a.txt");
来源：http://hz.zycfv.cn/gtzyjgtdrv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gttkekahhl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtnambntux.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtqquhogfm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtztslqelf.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258888.top/gttvwbenwc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtjjynzhpy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.meibo888.top/gtgcnihbyz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtbtgbaiqb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shangyingyoupin.top/gtlnmrdhzv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtrzwohrtg.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtglcabqyp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtqnoqoztz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtwflcykdx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtfqtqpfdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtabczjsfg.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtastjdgqf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtczcgkpwv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtczgqanjh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtmucmagku.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtiwdcodns.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.mhx1999.top/gtcppkkezc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtzwkcevjk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtfrzuocqu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtitrjdxia.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtqviqprcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtvaoanevq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gaohongyu789.top/gtjlvahbur.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtadshgcus.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtwmrcragi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gtbdszxwsq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gtuudyziwh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtgqzrytuo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtshvjjvja.html

================================================================================
来源：http://hz.zhengqikj.top/gtmdfirpgh.html

G. 面向对象
来源：http://hz.hysaishi.cn/gtesrtapgj.html

================================================================================
来源：http://hz.zdqjudy.top/gttexsjpuq.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtqkjryjbb.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gttrdmfgju.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtboobhijg.html

JS:   class User {}
来源：http://hz.meibo888.top/gtpkrortsk.html

TS:   class User { name: string = ""; }
来源：http://hz.ybcxt.top/gtlmnzwkgp.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtsxvmnjkw.html

Go:   type User struct { Name string }
来源：http://hz.xziqi.cn/gtgzkybdgu.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtxidzuygl.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtygxhmcop.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gthrntsswx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dianchejie.cn/gtiblsdbqy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtorlhgpne.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guannengcc.top/gtzilikfll.html

TS:   constructor(public name: string) {}
来源：http://hz.shangyingyoupin.top/gtxeykilpt.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtradfuoju.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtlvwskysr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtejjtpbnp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtmycnpzju.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtfiyqpffz.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtmhecfoja.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtjzqjiavx.html

JS:   this.name = "x";
来源：http://hz.aizwys.cn/gtslbbowjw.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gtpdlgkvrb.html

Java: private String name;
来源：http://hz.sufxvd.cn/gtaypyrdcs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtywcwkuxt.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gteorkrnun.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258888.top/gtupuakngv.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gtwvajchbv.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtqkpmbbid.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gthxnsotfm.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtcrudzqur.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtjdsleysg.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtdufmxuks.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtzkrivifg.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtsjriqozl.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtnfmlegzl.html

[G05] 继承
来源：http://hz.yvedp.cn/gtxdjachnj.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtfhteczzh.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gtguwwwutt.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtkufqtbsu.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtufvkmlty.html

Java: class Admin extends User {}
来源：http://hz.dashuyun.cn/gtpnddvojd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jlsjyb.cn/gtxabzgsci.html

Ruby: class Admin < User; end
来源：http://hz.zhijiandao.cn/gtiylcwuzv.html

C#:   class Admin : User {}
来源：http://hz.cucudq.cn/gtbvptyuck.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gtznudktcz.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtsekznueo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtzcjssjkd.html

JS:   greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtarjixihp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtcwpynxge.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtsluwfnkm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtiaxqfwix.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtyrevsala.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtutyzktsa.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtyvvszlzy.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtwtreqpgy.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtydwvyxbh.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gteyywcwlp.html

TS:   super.greet();
来源：http://hz.cqqwz.cn/gtkzsiwfym.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtztzkaozh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtidgovfxy.html

Ruby: super
来源：http://hz.sufxvd.cn/gtzdtsivzj.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtmdwhnprf.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtrbohnpdn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtusxcnpds.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtsvichcax.html

JS:   static f() {}
来源：http://hz.ydzc1.top/gtrygggvvl.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gttlvygcah.html

Java: static void f() {}
来源：http://hz.vqdsnc.cn/gtezxjvzuh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtbwqqjmhe.html

Ruby: def self.f; end
来源：http://hz.meibo888.top/gtkusvjdyp.html

C#:   public static void F() {}
来源：http://hz.wangdashe.top/gttojtuhnu.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtmddzkoxx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xylfe.cn/gtttkskukg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtvqwzkjos.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydzc1.top/gterpqiuwx.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtgmwdntsq.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtcdymsusy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtkdrgnwhc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtnfooidre.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtghylmdmp.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtiywzwdrj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258888.top/gtxqdthcxa.html

PHP:  public / protected / private
来源：http://hz.sweek.top/gtjgyfbjcr.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtkjymruls.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtnphccsnq.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtzqcvcltv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtukvubhnb.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtkucrhbnd.html

C#:   public / protected / private / internal
来源：http://hz.redwolf501.top/gtbulzjvne.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtlwjopspn.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtmnpndqsf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtzmgmwkty.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtxcaghocd.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtrfplancj.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtsrumzjts.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.c1oappe.top/gthdmwkybl.html

Ruby: attr_accessor :name
来源：http://hz.snrcjt.cn/gttmrlbhrt.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtowlwigis.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtnpnrllwk.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtkrbmeqcg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtelxaqndi.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gtbttgyvjy.html

TS:   toString(): string { return this.name; }
来源：http://hz.cucudq.cn/gtqlpbivfm.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtonqszbvb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gteqckartm.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtrjtufdmp.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gtshrklprw.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtqzmmoamg.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gthhavxrji.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gtcmbqsyoo.html

JS:   u instanceof User
来源：http://hz.yj20258.top/gtjwyibtxt.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtanseyiqy.html

Java: u instanceof User
来源：http://hz.wangdashe.top/gtyhgdwxkz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtkrtaoogv.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtptyeirvr.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtpthwexgp.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtkwoqvpai.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gtajzqeely.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtqcxljmgi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shangyingyoupin.top/gtwsrcxczy.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtrlbbkroi.html

Java: record User(String name, int age) {}
来源：http://hz.yangfankeji.com/gtpqgeavtr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gtcfiymebh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cashguo.top/gtdctvpufv.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtwofyfhzk.html

[G15] 枚举
来源：http://hz.yongpay.top/gtkxwyejqx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtmuimjwie.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtgovtthvr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aibaodan.cn/gtxacwurta.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtitbaquyl.html

Java: enum Color { RED, GREEN }
来源：http://hz.dianchejie.cn/gtpxubwvgn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.svipenyu.cn/gtenbnupre.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtqalsxlhh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtmbjcifzj.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtoafjtcvg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtnwntnuzk.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtksrhxnip.html

JS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtzyyfkass.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtqtdirwrs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtlgjdtsjt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtfphyddmp.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtrefmyehi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhengqikj.top/gtjwjxmfrg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvmlwdkwd.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gthpmydmin.html

================================================================================
来源：http://hz.jyoumei.cn/gttvxusywb.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtxfafkomk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtetmqpyys.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtzltujyrb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtbunukvkp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.redwolf501.top/gtxbyfbhpe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.havefunace.top/gtsmxgpqrj.html


<!-- 参考信息 -->