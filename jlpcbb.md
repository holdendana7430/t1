代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtgloukwsp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtkamegmvz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gtrjlpmxmw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gtdivpzuao.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xziqi.cn/gtbmzchyrr.html

[E19] 多行文本按行拆分
来源：http://hz.wangdashe.top/gtzfhzqndr.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gthmrtgbre.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daria6918.cn/gtpnhdrawv.html

JS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gthpztzpgc.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtwhtqqupl.html

Java: s.lines().toList()
来源：http://hz.bjfxy.top/gtqtnxkwjk.html

Go:   strings.Split(s, "\n")
来源：http://hz.dianchejie.cn/gtpsrbvxqr.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtrimdetus.html

C#:   s.Split('\n')
来源：http://hz.jinyuanbaomall.cn/gtknriuuag.html

[E20] 判断字符串是否为空
来源：http://hz.yangfankeji.com/gthixffgzo.html

Py:   if not s:
来源：http://hz.cashguo.top/gtiulxbgkq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhijiandao.cn/gtiewsfxew.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtfjcxdnsq.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtunrmqnkz.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtkiugajpj.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gtqufhqxve.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtmmtufwdw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258.top/gtpuhdnoqb.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gtzhjxnxgn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtiaxdegma.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gtizemxetp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtcqvewwkv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtdsdzjtda.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtfdhmiyui.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.quarkkingdee.top/gtbbvdyfbm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtybxxksek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtcdtzzage.html

[E22] 字节长度与字符长度
来源：http://hz.yongpay.top/gtkbrjsmyh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtcxyxnnwr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtokbjnoao.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtmjdnxnba.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gttycjemck.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tanke756.top/gtpmymzsnk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.52xcode.cn/gtqjsmxlnt.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtesiboaqf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigufen.top/gtvuuvxwbr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtscadpycw.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtafoxbgkc.html

================================================================================
来源：http://hz.zhongyouzk.top/gthzzuqqrb.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtbdrwpnop.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sufxvd.cn/gtwcwiwdwz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtzsidnvin.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xinyue.icu/gtawlinani.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gttktnvxrg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtxdvgorky.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtupeqbbha.html

Ruby: File.read("a.txt")
来源：http://hz.shangyingyoupin.top/gtndmitwmq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gtuzgnjnzc.html

[F02] 逐行读取文件
来源：http://hz.yj202588.top/gtjdotayna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gtmhswyeeh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aizwys.cn/gtfayluyvv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtluvvdrca.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtmesteaod.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtbknlpmps.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtllqtymhn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gtudtjyavq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtesepphhx.html

[F03] 写入文件（覆盖）
来源：http://hz.xinyue.icu/gtuavhtjni.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtjjozxdlp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtmffgfppr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtlkdjjory.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtdsirtokh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gtolibfomz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtbwqspfaf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtjgudqvay.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtfcqlytyf.html

[F04] 追加写入文件
来源：http://hz.ppjwa.cn/gtamxqilee.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtfwjadphr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cqqwz.cn/gtxtgacvwc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtpwwmdchw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtamrbyqze.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shzxlz.cn/gttjonurfr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtuecewyrr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gtgffgzllw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtuckwhptd.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtbrjztpgh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenjidiqi.icu/gtsxmgypbi.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtqopzapss.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gttujxobgk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gttyjbfvbm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtfafhwxvh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gogol.net.cn/gtfughwirt.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gthcrugqfu.html

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gtramvypsz.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtlqsaebwg.html

Py:   os.remove("a.txt")
来源：http://hz.gaohongyu789.top/gtgwimkxyj.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtagocdznn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtthqlouyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtxjwzdbtr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtrbfdwhxx.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtyltpvpid.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtassspjyq.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtgcpwizhj.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtskwmhftj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gtvgaufarn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtqugogqdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtdppupdfu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtmmdvamxe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fzhhl.top/gtdyeyfzjn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtppiryufo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gthdrjkjja.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gtsocxklbu.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtpqdpyhgr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtkemjsmqp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cheryme.top/gtysbhbkza.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtgqqnbqxh.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtjyxeolef.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtaboxjufv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtblhzsbgy.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtelfvgrez.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhijiandao.cn/gtfequxhwu.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtgdhkecvd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtosalfmqm.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gthjpxnemn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtbaxpzxne.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtfovkthbs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtlwegzltz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xylfe.cn/gtautitaac.html

Ruby: File.size("a.txt")
来源：http://hz.shzxlz.cn/gtkrcetrgf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258888.top/gthngshhad.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yanxiufei.cn/gtdtsaojxy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtihxbmrxv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gtqmkaxxna.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtggcakbob.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtexkgnryo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ehwqpu.com/gtruakpphp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yonumen.top/gthzceyqfe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtrqqvtmoo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtuolnqhqw.html

[F11] 复制与移动文件
来源：http://hz.yj202588.top/gtfmomfarc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtbxpobalp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.52xcode.cn/gthfppejpf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtwwedbasb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtxuwfpfkg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtaunpspbi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtignttoxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtzimtwbhf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.havefunace.top/gtgztdhzfo.html

[F12] CSV 读写
来源：http://hz.zhengqikj.top/gtrmmrddqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtkmoqyvvv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtfldagzxn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.52xcode.cn/gtzfijxhqu.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gttazctjzp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtuatuwukk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtrjaxeiog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tanke756.top/gtbzdqnsqz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtotyrzufb.html

================================================================================
来源：http://hz.c1oappe.top/gtioptipqk.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtemqnlsjn.html

================================================================================
来源：http://hz.yj20258888.top/gtwopqmgir.html

[G01] 定义类
来源：http://hz.yongpay.top/gtbtsywpbq.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtyklrsdut.html

PHP:  class User {}
来源：http://hz.redwolf501.top/gtanxvrpdl.html

JS:   class User {}
来源：http://hz.52xcode.cn/gtmyymzrbt.html

TS:   class User { name: string = ""; }
来源：http://hz.ydzc1.top/gtmtyowvai.html

Java: class User {}
来源：http://hz.jinqigfzy.top/gtxsrwxjvm.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtgscjbmkg.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtfgqvdkfq.html

C#:   class User {}
来源：http://hz.cheryme.top/gtgrfltcuw.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtquhypgnk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtyqovsvav.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtbfjcsfyx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtowdfafma.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtvrrsotek.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtbrftvask.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtgborphxc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtmohsqvdq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtyfhgsnfu.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gtyufbqaxl.html

Py:   self.name = "x"
来源：http://hz.haohaochexian.top/gtrmgyvsnx.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gtrdmprzis.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtfsxtgijb.html

TS:   name: string = "x";
来源：http://hz.xylfe.cn/gtygdxuhju.html

Java: private String name;
来源：http://hz.haohaochexian.top/gtbrghmdlu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtvxbehemx.html

Ruby: @name = "x"
来源：http://hz.kuanghao11.cn/gtzdcpoiig.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hongshengwenyu.top/gtqctdfjjz.html

[G04] 定义方法
来源：http://hz.iojbl.cn/gthzzitmjp.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtsqbwcplo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtzvtebmig.html

JS:   greet() { return this.name; }
来源：http://hz.iojbl.cn/gtfzkesteu.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtwxhswebq.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gtjhdizegg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtgtctqrnt.html

Ruby: def greet; @name; end
来源：http://hz.haohaochexian.top/gtelwbjxdn.html

C#:   public string Greet() => Name;
来源：http://hz.nanxinkj.top/gtsajifflu.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtomsddblx.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtrpdvrheo.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtuvbzonit.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtkvrvdbsv.html

TS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtcpxjmrtv.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gthfgtpsye.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tian-w.cn/gtwizdjaur.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtjewxlzqg.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtycincxuq.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtgwwtseup.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtiokfouhn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtghbiuqfh.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtplrhalfx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gttfojrzrn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtqbjqjwwn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pycfn.com/gtvrskihlx.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtbkxtvsqq.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtlyqnloxk.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtpxbrdxwr.html

Py:   super().greet()
来源：http://hz.havefunace.top/gtptuusozl.html

PHP:  parent::greet();
来源：http://hz.316326.xyz/gtnmfykdii.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtmsmjmcrz.html

TS:   super.greet();
来源：http://hz.andypj.xyz/gtdcqhwhtq.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtxxdqyhqv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtzpfxrhcj.html

Ruby: super
来源：http://hz.sxryk.cn/gtzvzbuxcl.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtdvwkfuyp.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gtknqsqfsm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtticekshm.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtscrtpdyo.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtdboneuqf.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtqhrgmmfu.html

Java: static void f() {}
来源：http://hz.xinyue.icu/gttzvxrdoc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtscyaayuq.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtznwgrmqh.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtgqqtedky.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtrxdtppcn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtphrnakop.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yvedp.cn/gtqmzggkws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuxming.cn/gtlgzoaejm.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtwsgvxngy.html

Java: interface Shape { double area(); }
来源：http://hz.shuidangran.top/gtfrsbxqab.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtwpqxffey.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gtsootvtek.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gtqoeubxbb.html

[G10] 访问控制
来源：http://hz.zhengqikj.top/gtorpzxfjt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gtbngmitfp.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtvmagiecw.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtklbcohyb.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtbzmvfifn.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtxapfbdig.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gtspdcduix.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtmsutxncq.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtdhuruxvs.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtobzurkpo.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gtwhsqfdff.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ivvv.top/gtbupjruex.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtoxgumtdp.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuanzhike.top/gtqozekxby.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtwvswwpah.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtmpfjpgvt.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gthsuljyug.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtsymhszoa.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtepydalxw.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtosoclncl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtuqyaxwwa.html

JS:   toString() { return this.name; }
来源：http://hz.chenlongwang.top/gtouhznwxg.html

TS:   toString(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtrnnmtumb.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuetiantiany.cn/gtumgkxelr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtwkwgtmpb.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtcgygnsxw.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gtpcahlpdb.html

[G13] 判断对象类型
来源：http://hz.nwbrower.top/gtcesujboi.html

Py:   isinstance(u, User)
来源：http://hz.cdnleiting.top/gtzitkozav.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtvimampxo.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtzfyezbej.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtqehpjzmn.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtdhzkeigr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtljpowawq.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtusmlogmk.html

C#:   u is User
来源：http://hz.daria6918.cn/gtwvmbeqrd.html

[G14] 数据类 / record
来源：http://hz.shuidangran.top/gtnkaezhrf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtizpndjwi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtjgqdrmgl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtcnyciokb.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtnxvoyqfg.html

Java: record User(String name, int age) {}
来源：http://hz.daria6918.cn/gtameuhpuz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtbpjvptxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtxizsryuv.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtkynzycsa.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtmwlljwyx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtnbuldyew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jiagoushi.top/gtwnqidfrg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtmzoimkqu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtsgxtbhsq.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhoulong.xyz/gtnjlsiyyu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtqxqewiyv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtjcnbmunt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtygysbjnn.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtmoohrgce.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hywenlv.cn/gtigbztknb.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtjllepqsx.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtsmpmnbfr.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtogsrvjnz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtyehqjncw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtoitssmpv.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtugafjkfz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtabmuxgdp.html

================================================================================
来源：http://hz.tanke756.top/gtakolcvhj.html


<!-- 参考信息 -->