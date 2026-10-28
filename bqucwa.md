代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.0kj1m.cn/gtybgrukav.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yonumen.top/gtjqrrvput.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gtolswiruh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtbjgssrmx.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtbxmsonfq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtqaozhjac.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgufenzy.top/gtqmiprqor.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gttqozwjio.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtjwhvrwir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtbsvzcsph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydjk.org.cn/gtgxmzgura.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtissfilkj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gtscismelp.html

[E19] 多行文本按行拆分
来源：http://hz.jinghuilouyu.cn/gtjeoamyrl.html

Py:   s.splitlines()
来源：http://hz.yuxming.cn/gtyonbgofk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gtfofkrzbf.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtdwbjdooq.html

TS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtarlxvfqf.html

Java: s.lines().toList()
来源：http://hz.cashguo.top/gtygufatwu.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtshhqqola.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtgdpkclmn.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtqncamqrd.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtykbzseub.html

Py:   if not s:
来源：http://hz.zhengqikj.top/gtffscukem.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xziqi.cn/gtidxchymi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtakwnpiox.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gthennaook.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtusulwkem.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gttlhmfonf.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtzrmjhnjf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtewycawrc.html

[E21] 超长截断加省略号
来源：http://hz.shuidangran.top/gthhlxtwmb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtyeqzgnov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydjk.org.cn/gtvfdwnbhb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtwskzafae.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtpwglqtdl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtkmwjiagf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xinyue.icu/gtjyldcbjt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gtlhddzkjg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.52xcode.cn/gtbwshjkvm.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtbougbeii.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhaomingkeji.xyz/gtelrjkftr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtjhavvfph.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtzufgtcur.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtvldjgguu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hongshengwenyu.top/gtnvywmfka.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gzhubu.top/gtddmdwbql.html

Ruby: s.bytesize;  s.length
来源：http://hz.yvedp.cn/gthxuvychm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuxming.cn/gthvfappha.html

================================================================================
来源：http://hz.yj20258.top/gtgvvuzvxq.html

F. 文件与目录
来源：http://hz.feifeiyinyue.top/gtcjpitcee.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtywaruoka.html

[F01] 读取整个文件
来源：http://hz.jinghuilouyu.cn/gtccgunjmh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgufenzy.top/gtpajfqaom.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nwbrower.top/gtydyuafis.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtkfagluqt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtprivffhs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtepkhfkok.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtjjvwhtfc.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtqheahaqu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gtthdotmvj.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gthlpgsxjl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtfnipudog.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yonumen.top/gtjwutbnae.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtpltcjaif.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtwlzjboeg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtrirhxejp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yvedp.cn/gtalfsjdef.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cdnleiting.top/gtsilxbbws.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yvedp.cn/gtavcljzrq.html

[F03] 写入文件（覆盖）
来源：http://hz.feifeiyinyue.top/gtqcjtjvlh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnxiangtu.top/gteduvpnwd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sysykeji.top/gtjxsdzfpu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gttbehnbcr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtdjcenghl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtizehcrdn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtaqcsxwvx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtcigudiny.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtoqhzyoze.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gthsiipwjh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtrvbmuzhf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zycfv.cn/gtgeugswbb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtefnzyccx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gthubpcndu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gttjnsjygf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtontlhbvq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhongyouzk.top/gtjndcxftb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pengpengdd.cyou/gtupstlaqy.html

[F05] 判断文件或目录是否存在
来源：http://hz.cdnleiting.top/gtlarmsfww.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtcgeufuaf.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gtnvzoxcpe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtksxmvaug.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtnlmswlxy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtjdapnzox.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtneqteneh.html

Ruby: File.exist?("a.txt")
来源：http://hz.yongpay.top/gtgpghkutc.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258888.top/gtsfnosprj.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtjaltuibe.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtvokulygu.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtdzbhnymm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtsjqnwvfg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gttnrabluq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtlvrsyvua.html

Go:   os.Remove("a.txt")
来源：http://hz.guannengcc.top/gtuhqdvjqu.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtwfzmpyvk.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtmmltyaew.html

[F07] 创建目录（含多级）
来源：http://hz.zhixingplan.top/gtptsfjnlg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtecilceqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gteczscaoe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtpwliekpo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtlgrnmqcl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gtomwnfbpy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gtojuxtzyq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gtfvdwlonk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.havefunace.top/gtaupsllch.html

[F08] 遍历目录
来源：http://hz.chenzaomai.com/gtynxkabwn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtytjnrcye.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtkmxawgba.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtonufzemx.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtiehzrkuz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtvlnqxwcx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gtdxnlescc.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtcwkajrtp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtabweagso.html

[F09] 获取文件大小
来源：http://hz.xziqi.cn/gtpuswvhrc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gtygvpsnnf.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtbqbvbivx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtwxfpqlcw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtlpgpoici.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtopalwqsh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aibaodan.cn/gtziqtzjyo.html

Ruby: File.size("a.txt")
来源：http://hz.iojbl.cn/gtdijdjmie.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtzqzsaxdd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtozamfhun.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtterpbuwa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gthgxbpqpt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtipfhpcll.html

TS:   path.extname("a.txt")
来源：http://hz.haohaochexian.top/gtgvdxvbrr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtrofrgucf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gtsrplyxfl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtsxgahdxc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gttzeqolbg.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtnngxlcsb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtxpcndzvd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gtvieuikwk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtwalaoptz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtiugablrx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtcxzayelv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gtoqnayuzu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gttpwttltl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtkyajghsd.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtywbmhctg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtddkwbxmi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgufenzy.top/gtogusivxu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtbxrclvej.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtaleybhoi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gthvgqzhid.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtggaxbfxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtdmihmhyi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gtrldtglub.html

================================================================================
来源：http://hz.cheryme.top/gtgbpsifhr.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtzyflzfvu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxxfqmkvh.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtjqpsoqqc.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtklwppzsv.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gtvhakebhu.html

JS:   class User {}
来源：http://hz.iojbl.cn/gthxmuhqsr.html

TS:   class User { name: string = ""; }
来源：http://hz.fengsongda.top/gtelpzhomd.html

Java: class User {}
来源：http://hz.quarkkingdee.top/gtwtfnujhi.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtbsleuclv.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gthkvtalpt.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtclqducnq.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtbyzlfgky.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dashuyun.cn/gtthrluwrr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtegactkxz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnqzz.top/gtiashaukj.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtvuvbxigl.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtmxwnrets.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.birdmap.top/gtnwyvjuwt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xylfe.cn/gtcpdjpgyw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtbgttvvwz.html

[G03] 实例属性
来源：http://hz.cashguo.top/gtsuaudgik.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtvgudnwfz.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gtrunhwlrf.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtjitcitcw.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtnuupuain.html

Java: private String name;
来源：http://hz.tanke756.top/gtuvwflnaq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgufenzy.top/gtfvygloqk.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtkdherwoi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ehwqpu.com/gtrtqgajzv.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtcobxzibk.html

Py:   def greet(self): return self.name
来源：http://hz.wangshuangyany.cn/gtibwcmtib.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtpchzpsuw.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtigsahyps.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtinyrkbqo.html

Java: String greet() { return name; }
来源：http://hz.tianlin.xyz/gtzvnxmszo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuxming.cn/gtmsoauruz.html

Ruby: def greet; @name; end
来源：http://hz.jyoumei.cn/gtrwotzdiw.html

C#:   public string Greet() => Name;
来源：http://hz.fengsongda.top/gtynedykdl.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtqzpckrwe.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtnykrmpcx.html

PHP:  class Admin extends User {}
来源：http://hz.xziqi.cn/gthqipbykg.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtsgubwsoa.html

TS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gthyrgikmg.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtvqxfaqui.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtnbufityx.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtoytruqax.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtpnfefkmw.html

[G06] 重写方法
来源：http://hz.yj202588.top/gthzrlahby.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtxzzrjgau.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtygcaoawk.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtuhikgtyb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtgrydompf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtglcotneq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtxrlzwnkl.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtnbqupjyi.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhongyouzk.top/gtmakvkvvy.html

[G07] 调用父类方法
来源：http://hz.gotoacloud.top/gtuvcbgclu.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtoutvwwoy.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gtjwtlkrrf.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gtnugssdjh.html

TS:   super.greet();
来源：http://hz.guowangkeji.top/gtbtclsexf.html

Java: super.greet();
来源：http://hz.cqqwz.cn/gtuxffaqma.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtlfymwmfy.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtmqbzktyw.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtpsjriphn.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtvntwafzd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xinyue.icu/gtwzjvysty.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtboeshonb.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtjmfaobdv.html

TS:   static f(): void {}
来源：http://hz.zhengqikj.top/gtmqbifhjc.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtnoglqrpp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.316326.xyz/gtekoewmfw.html

Ruby: def self.f; end
来源：http://hz.yuxming.cn/gtgcgdnfnf.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtasbdknrz.html

[G09] 接口 / 抽象类
来源：http://hz.zhoulong.xyz/gtynendzcu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtwjazzdaq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tian-w.cn/gtwsdgfzig.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigfzy.top/gtnuiqmonn.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gtkppajwbm.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtiqjbcybn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nwbrower.top/gthlrdswff.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtjtctnuas.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gtgomxgqan.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gtxbtxydoa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtywtgzlww.html

PHP:  public / protected / private
来源：http://hz.ybcxt.top/gtdggubbyp.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtmlvdnnqi.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtjcskkrdc.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtaigfxxhx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shzxlz.cn/gttmbjqhsy.html

Ruby: public / protected / private
来源：http://hz.svipenyu.cn/gtvgefxnzt.html

C#:   public / protected / private / internal
来源：http://hz.jinghuilouyu.cn/gtltldvqkj.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gtzctfthpz.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtfxenbslo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtsvahmtdk.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtzhpayewt.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtrzvvnmdd.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gthbhpzxks.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtvyhpeqhs.html

Ruby: attr_accessor :name
来源：http://hz.xingfuxueyuan.xyz/gtgbwrabep.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gtpnagzwhf.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gthzfubcnk.html

Py:   def __str__(self): return self.name
来源：http://hz.jlsjyb.cn/gtplduhrpg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtooyzzctd.html

JS:   toString() { return this.name; }
来源：http://hz.hfpthk.cn/gtqvvjayln.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtqqmwagds.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnqzz.top/gtxmjjfoww.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtxdjnvphy.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtnvjnviyf.html

C#:   public override string ToString() => Name;
来源：http://hz.yuxming.cn/gtdpzpwhrm.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gthgzwwpeq.html

Py:   isinstance(u, User)
来源：http://hz.sufxvd.cn/gtmxqeueys.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtszryrdsa.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtvhesukeu.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtsaybtgbt.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtunqflnem.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtacjrqakh.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtvndwmvmh.html

C#:   u is User
来源：http://hz.yj20258.top/gtteoqhiuy.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtysvvcdha.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenzaomai.com/gtafhyrfcx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtywqeyosr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gtfjyiizct.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gthujzfzoz.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtgickxiii.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtpiavtnad.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtltioxdgy.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtjupoeaoa.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtwfhtdlea.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtwzlzcoov.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtqzgodjnk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtnkgbjphh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtednvrkls.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtuscaqwiu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtvrsxkykb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jianghu66.top/gtfwotlfey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtzycwqsto.html

[G16] 对象转数组 / 字典
来源：http://hz.yuanzhike.top/gtsviesvrf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xylfe.cn/gtiseapbfl.html


<!-- 参考信息 -->