代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhixingplan.top/gtgrpftslm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tianlin.xyz/gtjbhhdkja.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtnnmrxohv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtzzatfmrw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtiulagqzf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtyitejnqi.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtbvopsprr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtzevoentu.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtpixdbvvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daria6918.cn/gtitygompb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hammf.cn/gtuuwtnens.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtamcundlz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtbhmjhwey.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtpbsgpixb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gtpmcjcjod.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtlzqnjlip.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtjajkamrk.html

[E19] 多行文本按行拆分
来源：http://hz.yanxiufei.cn/gtwcthfwfr.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtflkbiscy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigfzy.top/gtnsxfzpab.html

JS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtiybvmpfy.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gticglbypt.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtdcncdhmr.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtlflccivv.html

Ruby: s.lines
来源：http://hz.sufxvd.cn/gtmfdnhakq.html

C#:   s.Split('\n')
来源：http://hz.ydzc1.top/gtgrfavxmj.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtkjmurcff.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtcjyabmpu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hfpthk.cn/gthklryehd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ivvv.top/gtdwkszrae.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtpquzvckt.html

Java: if (s.isEmpty()) {}
来源：http://hz.mhx1999.top/gtigdfzyhx.html

Go:   if s == "" {}
来源：http://hz.cqqwz.cn/gtoyxpywve.html

Ruby: if s.empty?
来源：http://hz.sweek.top/gthcianzkv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gtcmbvlazz.html

[E21] 超长截断加省略号
来源：http://hz.xylfe.cn/gtebckzmtx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sufxvd.cn/gtgzaclcih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gtvmacbvzk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtenvyacse.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtsikccdmi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtmfdmbdpp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258888.top/gtuetxwvbp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnxiangtu.top/gttyfxdxis.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtfitahqbp.html

[E22] 字节长度与字符长度
来源：http://hz.sxryk.cn/gtlqkulanw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gtxvzakiao.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtmtpnhxjm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtjwjserkw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtalfoudaj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnxiangtu.top/gtitpamrmb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aibaodan.cn/gtcrurjfdp.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtvaxbbpod.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxinkj.top/gtyevauzcq.html

================================================================================
来源：http://hz.quarkkingdee.top/gtuqchxton.html

F. 文件与目录
来源：http://hz.daria6918.cn/gtctdqtchq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwhqvwaxs.html

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gtupgajpjp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ehwqpu.com/gtfeliznfx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuanzx.com/gtsiwvblxd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xinyue.icu/gtdhfzvvkk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtusuqbngx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtocroracf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sxryk.cn/gtyopvzxiq.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtkzyguobo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtbvmqvyod.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtgoaixrpp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.haohaochexian.top/gtrhoheodn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yanxiufei.cn/gtkdsxgowo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtngfwmidb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtthbldfou.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtsjrgtxym.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hongshengwenyu.top/gtwtharxir.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tanke756.top/gtzwzbndwf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gtanleyafa.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtodpjfxjd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtbpxbsejc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtyvhlqbpq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtwbqvxogv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtcxrjsqym.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtuosxldev.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtflgztluk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gtdfoijqwj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gttrobgsom.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtbwobqulm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangdashe.top/gtggojhfvi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtssmaznee.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtgzlbxfci.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtlyntvexc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gthwxwxprc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtiddndeoa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtapcnqngj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtryjabfkv.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtrbugpjwv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gtiyvrpdci.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtnafxfsei.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtoinvtkcy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtweiwsfus.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtgyjdmecc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtyqkirqei.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtuqglflzs.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258.top/gtfndrvvtm.html

[F06] 删除文件
来源：http://hz.yanxiufei.cn/gtixfwqhnx.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtkantdnwp.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gtuuzmjekp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtcqgijldl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtpctpqfzb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtkuaydmrp.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtqempkmzm.html

Ruby: File.delete("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtihdidcvk.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtrrwpakhv.html

[F07] 创建目录（含多级）
来源：http://hz.yvedp.cn/gtxrkaktnw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xinyue.icu/gtkdzchgmy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xingfuxueyuan.xyz/gtkurxhxgp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtfsnwjykn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtljgzmcxc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuxming.cn/gtijefvufz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gtczfbbpai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtjjqiptbm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gtghpyaari.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtxttiveud.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinyuanbaomall.cn/gtgjbyxxxd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtfoaoqymm.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtxuhwpxhn.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtfutateod.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtuuftpzfx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtnjsnbsnf.html

Ruby: Dir.children("dir")
来源：http://hz.yangfankeji.com/gtswupdgca.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xingfuxueyuan.xyz/gtqonvgvkv.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtmzcvvkqr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtivfbwtub.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtciucogil.html

JS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtjnygyewe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtlmnhqann.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtrizdesoo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cqqwz.cn/gtfuujuczn.html

Ruby: File.size("a.txt")
来源：http://hz.jqgufenzy.top/gtebrenjst.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sysykeji.top/gtiqocgyaq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtutgmupri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtsibxicgr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtgmdyanll.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtkwunmpll.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtpgmpsldx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtckdeuoii.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtrgrfrecy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtwkbfjrtr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guowangkeji.top/gtlyjjzvkc.html

[F11] 复制与移动文件
来源：http://hz.c1oappe.top/gtxydumzfz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtsnvdufvm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gogol.net.cn/gtsnhxdmdn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtvitalntm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtizktxpqz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258.top/gtzfsbaotn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtnhoyabdx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtoatmhdku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gthktmclsj.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtssqqolua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydzc1.top/gtcmqsfnze.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ywan-chungtsiang.top/gtjtxvwmcs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtnkpmxvui.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtsqyycnut.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtbbahlmnm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtxsiihepp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtlxvbfbzd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtybquydhd.html

================================================================================
来源：http://hz.cucudq.cn/gttbyscxlu.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtybwltmzh.html

================================================================================
来源：http://hz.tian-w.cn/gtbintyvdd.html

[G01] 定义类
来源：http://hz.birdmap.top/gtffwxzabd.html

Py:   class User: pass
来源：http://hz.cucudq.cn/gthuzwrqah.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gtvglfudlp.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtneeahqlh.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtgfhcvglx.html

Java: class User {}
来源：http://hz.pengpengdd.cyou/gtxaedlxjx.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtyqvhrtef.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtjtjoumca.html

C#:   class User {}
来源：http://hz.iojbl.cn/gtvdqaxijl.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gtrwhdgpkz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pycfn.com/gtmgenvrfm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtsuuvozae.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtuhmttpjq.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtaslokhpa.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtqyzhigcz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtyvujbmqo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gtvvtggcjh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtdvzyalen.html

[G03] 实例属性
来源：http://hz.316326.xyz/gtlvdsxdmg.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtxqnwlyjs.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtxxsiqzdv.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtdnwqlley.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtxoarplvy.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtpemovuju.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gtpnnyvpcl.html

Ruby: @name = "x"
来源：http://hz.jinyuanbaomall.cn/gtulnamndz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtsbwuryge.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gtakyyvbzj.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gthxfepwre.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtcaiijqru.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtdqwicwxg.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtevpzaric.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtmbrioaic.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtosksqegs.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtgebxfsup.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtljdojdvv.html

[G05] 继承
来源：http://hz.shzxlz.cn/gtwfnolkih.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gthxgofxsj.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtcgmyjeif.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtqiupphms.html

TS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gthalttdqv.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtcseeukhb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhaomingkeji.xyz/gtqtcblagw.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtoezkczfj.html

C#:   class Admin : User {}
来源：http://hz.snrcjt.cn/gteigknadn.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtmuqznlhi.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtifeiqkaz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtjtuqducb.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtwzednciu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtzsqmzunn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtfdxzxftk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gttbxfzrrt.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtxfznekaq.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gtmaawepar.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtiyxfhzpe.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtujpovaig.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtmlnlstwz.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtowgbixvr.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtrtoqysue.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtuhbecayh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhaomingkeji.xyz/gtmeizymph.html

Ruby: super
来源：http://hz.yongpay.top/gtznfixyzu.html

C#:   base.Greet();
来源：http://hz.nwbrower.top/gtxfneinip.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gteaglnxls.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.0kj1m.cn/gtpwfxcvot.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtpgqonbru.html

JS:   static f() {}
来源：http://hz.xuanzx.com/gtomtxkpln.html

TS:   static f(): void {}
来源：http://hz.nanxuanxn.top/gtcqzjmmpb.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtjrtbkyzc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtpyejkyvr.html

Ruby: def self.f; end
来源：http://hz.yanxiufei.cn/gttyfdxxaq.html

C#:   public static void F() {}
来源：http://hz.chenjidiqi.icu/gtghgdhgqo.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gtlxzesqkb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtgfemrwde.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gtmkptdygd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gtgifbluqz.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtkadiwewm.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtzrqpqlol.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtmjbbcddk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shuidangran.top/gtujoslwyq.html

C#:   interface IShape { double Area(); }
来源：http://hz.redwolf501.top/gtfvdkekjh.html

[G10] 访问控制
来源：http://hz.316326.xyz/gtxmlffahq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtmyyplyso.html

PHP:  public / protected / private
来源：http://hz.jyoumei.cn/gtekpmeuxk.html

JS:   #private 字段；其余公开
来源：http://hz.sysykeji.top/gttdbypnzf.html

TS:   public / protected / private
来源：http://hz.birdmap.top/gtgcgohhzu.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gtdymwlyey.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtkafmtenf.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtpnrdwonn.html

C#:   public / protected / private / internal
来源：http://hz.cashguo.top/gtpdhksuol.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gtnhorwbew.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtqzgmwyzt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtkvvmraer.html

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtlnwcirds.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtydbsvdiu.html

Java: public String getName() { return name; }
来源：http://hz.yonumen.top/gtaitdamhm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtprmltptp.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtkxkpeanh.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtuuvphrte.html

[G12] 对象转字符串
来源：http://hz.nwbrower.top/gtgltmeyls.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtsnhxbkqg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gthmsqdaen.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtbkvrxdrl.html

TS:   toString(): string { return this.name; }
来源：http://hz.bjfxy.top/gtwvjzhhze.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtviwzgdej.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtnqkzrdqb.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtsufjsdks.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gtpwmctlzz.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtprhybybo.html

Py:   isinstance(u, User)
来源：http://hz.svipenyu.cn/gtwoepsszd.html

PHP:  $u instanceof User
来源：http://hz.chenjidiqi.icu/gtsmlftfyn.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gttlbnnibl.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtbulcxpfj.html

Java: u instanceof User
来源：http://hz.zhoulong.xyz/gtkyugikve.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.9152youxi.cn/gtscfuebwz.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gtkmhetuen.html

C#:   u is User
来源：http://hz.smart0.xyz/gtmhuljpkh.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gthuyvrufb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtgytoirzb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtbwomixwk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jiagoushi.top/gteiitrumz.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtzpbessby.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtdpbhaukw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtbnaxqfji.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtrjkwbsht.html

C#:   record User(string Name, int Age);
来源：http://hz.hnxiangtu.top/gtskywnamo.html

[G15] 枚举
来源：http://hz.andypj.xyz/gtcvmxnnrp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.vqdsnc.cn/gterrcfekj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gteaclapgj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zdqjudy.top/gtlzdtmqkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtbjtozbxt.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhongyouzk.top/gtekdtolbl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtytvdasnf.html


<!-- 参考信息 -->