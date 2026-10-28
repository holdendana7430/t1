代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtuptxtuaj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtjmfqurlo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenlongwang.top/gtiwhzgvhx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jianghu66.top/gtiqyuxfpr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigufen.top/gtwqpactzx.html

[E19] 多行文本按行拆分
来源：http://hz.svipenyu.cn/gtribotrch.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gthpgbzreq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.meibo888.top/gtjjmimuzz.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtrgcxlrjw.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtlbifbrsv.html

Java: s.lines().toList()
来源：http://hz.guannengcc.top/gtnvdimksm.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtvluethyh.html

Ruby: s.lines
来源：http://hz.fengsongda.top/gtfkqpiyky.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtialbtsup.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258888.top/gtarfwjoyj.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtusntemed.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zycfv.cn/gtyrvkjmfj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yueranfly.top/gtjjyqkzkb.html

TS:   if (s === "") {}
来源：http://hz.fzhhl.top/gtzjnqwshj.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtmejimqhf.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gtueadocbk.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtdewdhvfw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgfzy.top/gtxmcvjwyi.html

[E21] 超长截断加省略号
来源：http://hz.nanxuanxn.top/gtygyfdrgr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gtrojbbiby.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gttunupkbw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtxxirsmof.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtopzksevo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtsmznygtg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xingfuxueyuan.xyz/gtmwwhfoum.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtedllycel.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtphrckrjh.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gtmclydius.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtvtxafctm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtnzkfaotu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gtsxrblhkc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtqgaqndxe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gttseplslp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yonumen.top/gtphqxajau.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gtbtxhlmtm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtenkmusxe.html

================================================================================
来源：http://hz.sysykeji.top/gtfeuuigrg.html

F. 文件与目录
来源：http://hz.tian-w.cn/gtxjrzvfyy.html

================================================================================
来源：http://hz.tianlin.xyz/gtsvevlryb.html

[F01] 读取整个文件
来源：http://hz.ivvv.top/gtfbszzdxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtbotqbxsx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtlyshueyd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtytyrznaq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtwkanssot.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtjxsfdqzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtoyrkwcgm.html

Ruby: File.read("a.txt")
来源：http://hz.iojbl.cn/gtqxafolgj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtzqfdbcpq.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gthwltmyyc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gtnscyklwk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhijiandao.cn/gtfyusjztp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtpxhiufvz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gtqqbiseqh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtfxjonrjh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yongpay.top/gtusjnwuqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhixingplan.top/gtrsvkjwpb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.0kj1m.cn/gtonrthiak.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtibinnaxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jiagoushi.top/gthurwaptn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtuehxcshn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtyjxdewit.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtfqeyoeej.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guannengcc.top/gtvtvmlpob.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gtirwiqlcx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sysykeji.top/gtrddfvuxd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ivvv.top/gtrfulgtaf.html

[F04] 追加写入文件
来源：http://hz.sxryk.cn/gtxpututyu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.iojbl.cn/gtbzvuudsq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigufen.top/gtvzbzzsbs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hysaishi.cn/gtsprniwde.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtbtopvcuy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hongshengwenyu.top/gtfqsjldbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtlejhehhc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtlserhert.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtgvyiqdql.html

[F05] 判断文件或目录是否存在
来源：http://hz.havefunace.top/gtefmcsqiq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gtvfhfcxei.html

PHP:  file_exists("a.txt");
来源：http://hz.hnqzz.top/gttgqupzbl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtapfirapf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtqcxhapae.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtanwqqgud.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ywan-chungtsiang.top/gtklhlzvbg.html

Ruby: File.exist?("a.txt")
来源：http://hz.havefunace.top/gtodvxvljn.html

C#:   File.Exists("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtavxyudpl.html

[F06] 删除文件
来源：http://hz.ybcxt.top/gtjsipyncg.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtfdnocsls.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gttjdgroiq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtxzdmhazd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtgcbdwqqk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtwmmcoipn.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtiwejkwvm.html

Ruby: File.delete("a.txt")
来源：http://hz.pengpengdd.cyou/gtpflludzn.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtlwolzutg.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gtzsoeqmbf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gtliufyuum.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtwibrrvaz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtjmpbfiof.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtgcqowlyx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtrfbzebqo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gtstuxfmmi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhiwuduotai.top/gtaglbfows.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtlyyrncap.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtsbjrvxkc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gzhubu.top/gtcebbdxfg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuxming.cn/gtedngwpqe.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgufenzy.top/gthtiwyris.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtlwcjgmob.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtlvthakxv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtkrwsevgh.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gtiojhhhkv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtbxptokbi.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtklkeouej.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydjk.org.cn/gtodzwmybi.html

PHP:  filesize("a.txt");
来源：http://hz.jqgfzy.top/gtbfnkclgw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtkokbndkc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtzkioqzfh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtnhhafjjt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtvpnprbcx.html

Ruby: File.size("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtamnohgpd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtroncvvco.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtneckiael.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtdmpnozck.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtqyzqjfkg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtznvlesvo.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gthonnftji.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtfdpkfxhs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtmfhcoymz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtydcayqlg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtklaolmfh.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtrmyjinjn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtmqcewcne.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yuanzhike.top/gtxhiomsoy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtorirpcqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gttmcvrsuz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtpkhytqic.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinyuanbaomall.cn/gtipuehbkf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gttlrzqwit.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtjxwxweye.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gtjxwhqmbk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daxiang520.top/gtllkmoxks.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtfrgzclbz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtxqwvzdph.html

TS:   // 同上
来源：http://hz.hammf.cn/gtzowvwoww.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtrchwhrbj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtdljnufbf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gtqmrkbwea.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtmansrufo.html

================================================================================
来源：http://hz.xinyue.icu/gttnefjkni.html

G. 面向对象
来源：http://hz.pycfn.com/gtaunvpqkn.html

================================================================================
来源：http://hz.zycfv.cn/gthcmlvqox.html

[G01] 定义类
来源：http://hz.andypj.xyz/gthdljxjuj.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtasjbubpw.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtlehzxtvs.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gteaztkojn.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtjygelbnw.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtkhzxhjhv.html

Go:   type User struct { Name string }
来源：http://hz.yuanzhike.top/gtklrevzdt.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtzyombpxj.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtwwmvtmck.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gthkwjuiyw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gttrontbdb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtyrcrfmfz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtwhhcnlqa.html

TS:   constructor(public name: string) {}
来源：http://hz.zdqjudy.top/gtjwmdcdea.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtnonbkpsv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtskjfcdqm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtsenumdhl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtmwqriivt.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtfgrdudat.html

Py:   self.name = "x"
来源：http://hz.ivvv.top/gtxyrpphce.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtyussxyfw.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gtaeragisq.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gtykqvnaqu.html

Java: private String name;
来源：http://hz.jinghuilouyu.cn/gtnodnumda.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gttkdcwweq.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtgeyoxgla.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gttjkizist.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtyomsftfy.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtgirhorme.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtdwndozuf.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtisonqdnf.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtqpilkwss.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtsvrhruad.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtjmnxloty.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtairxwjjo.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtbgfvutgm.html

[G05] 继承
来源：http://hz.snrcjt.cn/gtiinmfney.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gthfyodols.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtmduwctev.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtxlchdvdt.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtjnfluyzg.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtyrxjcxdh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gtxgwcilwj.html

Ruby: class Admin < User; end
来源：http://hz.dianchejie.cn/gtqdtxgtsd.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtdqppjuym.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtvofbccqp.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gtiilgvlrt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtfjhuhspo.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtbcdtwwky.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtgudsytun.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gttrmkbxfk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtsheikodd.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gtuzuqttly.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtrkhlgfvi.html

[G07] 调用父类方法
来源：http://hz.andypj.xyz/gtyorzyemy.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtphhsuole.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtcmskrswn.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtldplbhxa.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gtaaqthmgi.html

Java: super.greet();
来源：http://hz.meibo888.top/gtsjuwedps.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangtech.top/gtlrouzomw.html

Ruby: super
来源：http://hz.yangfankeji.com/gtatlkqxsn.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtbtiavuae.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtraqfuohw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtojptlnkv.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gtthkozghu.html

JS:   static f() {}
来源：http://hz.ywan-chungtsiang.top/gtxmptzkli.html

TS:   static f(): void {}
来源：http://hz.52xcode.cn/gtwghdrxvn.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtgtkkhqcu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zycfv.cn/gtuhagzewm.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtwlnbsiio.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtsiqdlhob.html

[G09] 接口 / 抽象类
来源：http://hz.cucudq.cn/gthbofhdrb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtxyheumbu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gthdamqzgi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gtocdolzrg.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtjjbofafa.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtvywrklyn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtbceqnvjj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtxwpfrtrx.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gtzlimexcc.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtkonxmnnt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtzblyfvkq.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtbugvppky.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtinyevxxe.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtabchmlsd.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtddkjeulm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtjuosmmrk.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtyulggiri.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtiglprpwb.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtsyksexno.html

Py:   @property 与 @x.setter
来源：http://hz.gaohongyu789.top/gtugjsrxen.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ybcxt.top/gteuirdkgi.html

JS:   get name() { return this._name; }
来源：http://hz.yongpay.top/gtyodhweva.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gteclhzbqb.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gtejfymbnx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shzxlz.cn/gtqbhfxkao.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtugyrznrw.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtwlzjljet.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtkkbrcfzp.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtmwvybkce.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtvgjqamgk.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gthbondysw.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtbpwitjjh.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gtkqocqbrv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gthdcmaszd.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gtsqpczllj.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigufen.top/gtzutumusv.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtnyogxdow.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtjojwchgo.html

PHP:  $u instanceof User
来源：http://hz.svipenyu.cn/gtlondncmi.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtrtepoets.html

TS:   u instanceof User
来源：http://hz.xziqi.cn/gtwdwerxsr.html

Java: u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtlgvjuiis.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtpxtaxbfl.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtqkhwuzdh.html

C#:   u is User
来源：http://hz.pycfn.com/gtxbicrpkw.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtomhpkrhp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtncevapbu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gtvolqyqjk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gtzvvtoreb.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtgaikqbsw.html

Java: record User(String name, int age) {}
来源：http://hz.yuxming.cn/gtrbzhagjm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gtbepmdmxd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hfpthk.cn/gtbrgnrxvy.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtsuwkuauu.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gttzewbmcb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtnqwevtrw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hysaishi.cn/gtcboxawax.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtinplafjd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtqwayxeyh.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtsyyorrcn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtqpwpnpfj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtfhjpymag.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtqkhxvpnh.html

[G16] 对象转数组 / 字典
来源：http://hz.gaohongyu789.top/gtrbpqqueb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xylfe.cn/gtqhnkngsh.html

PHP:  get_object_vars($obj);
来源：http://hz.mhx1999.top/gtomypublf.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtlaqgcwzg.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtpzzizagz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jyoumei.cn/gtqwgvvqbk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gaohongyu789.top/gtedrxfpim.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtyglodxur.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtddjcwfqn.html

================================================================================
来源：http://hz.hammf.cn/gtwiqneeei.html


<!-- 参考信息 -->