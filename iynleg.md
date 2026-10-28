代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gtjstjnhjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtyftunses.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gtycitmdxh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtzraxqjwl.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtrvpomkip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gtelddrskn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.kuanghao11.cn/gtuwhqgrni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtlgnbviqe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtducqebzr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gtezvsfpjg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtxovhwyiz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgfzy.top/gtxzwttjei.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtizphchmw.html

[E19] 多行文本按行拆分
来源：http://hz.jinqigfzy.top/gtmuxthurq.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gtppewbnwf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtukpstyrv.html

JS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtfmpytxiw.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtdzzijdac.html

Java: s.lines().toList()
来源：http://hz.sufxvd.cn/gtfvoovgfs.html

Go:   strings.Split(s, "\n")
来源：http://hz.zdqjudy.top/gtzrkmvfyq.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtwelubjgg.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gtwpjjzsyl.html

[E20] 判断字符串是否为空
来源：http://hz.9152youxi.cn/gtagjkbldu.html

Py:   if not s:
来源：http://hz.jqgfzy.top/gtqqsynask.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtqeotoftm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guannengcc.top/gtcnlsemmh.html

TS:   if (s === "") {}
来源：http://hz.pycfn.com/gtpmnaqvbm.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gttnpcuzks.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtylzdsbng.html

Ruby: if s.empty?
来源：http://hz.haohaochexian.top/gtuszscijb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.havefunace.top/gtrqqavfeo.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtvedeipyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtthqrcmyn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tanke756.top/gtqpcrrpqg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtmgojrubz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtrsmlmios.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtvirzjmqm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtrjdukmos.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtxtbcfsvy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtysdofeto.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gttjizzree.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigfzy.top/gtfelnpquy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtivlmxhni.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtfllfcvth.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtqhccbtai.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.havefunace.top/gtkiekxedo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gttuxsgqlf.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtvpxhdejx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtuozqlxsb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttrvanemn.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtslwdkvli.html

================================================================================
来源：http://hz.zhijiandao.cn/gtazhekdqf.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtgfmzsbhl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtbqmkpxzk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hammf.cn/gtgqujmnuh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangtech.top/gtydlwiikl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtohbktqjw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtdunimdiz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.316326.xyz/gtlfhamwhw.html

Ruby: File.read("a.txt")
来源：http://hz.hnqzz.top/gtxzzxvxgu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gtiqxzmmoq.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtkvudiszz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtenofdpvs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.vqdsnc.cn/gtybudoqgn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtncftnvam.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtshjnqaug.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtvdjhcfzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gtaowfbrin.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gteuctsxcw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxinkj.top/gtcqhpiack.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gtemovcwhn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangdashe.top/gtglftzpio.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtxidhihss.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtlcivjjes.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtpmlwefea.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gteltrxkxu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuanzhike.top/gtiiyfqmwt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ivvv.top/gtzxwseayz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtjkmevjgb.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtrqtwzlho.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtlrlpvjqx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhiwuduotai.top/gtbutjfzxk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtzebpgkbm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtnmlpqiqg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtihmofpar.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtgyjxomrw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtuxvcgzkq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtfqqmuvnv.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtmytfmsyn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.snrcjt.cn/gtevxlnwce.html

PHP:  file_exists("a.txt");
来源：http://hz.xylfe.cn/gtvyehwgmq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtwuhcvhpz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtosajxxsa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtqaamhocw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtvpqwxlot.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtlsybodqh.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gturxswlui.html

[F06] 删除文件
来源：http://hz.0kj1m.cn/gtnytulbuv.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtraagllxv.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gtqtmcbpdx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtnpuzaple.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtzgwudbmf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtjyanrbpt.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjumrapuq.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtlkftqctt.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtcwfmwect.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtrftcvgjm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtjijyyqys.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhoulong.xyz/gthiuodjhv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtkihpuvcb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtfiedqmnn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cqqwz.cn/gtjtstfhrk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.meibo888.top/gtbvdgxcrn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtvzxrchhh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtjzftgddg.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gthrtaplpc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtxwutkgtz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtznwrworo.html

JS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtcnpahcew.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtjpcdawkq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtipcwvswy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinghuilouyu.cn/gtueglhevz.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtgxqthcrq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtbggkotuw.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtkywafgxg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtziuewqkm.html

PHP:  filesize("a.txt");
来源：http://hz.tianlin.xyz/gtdpaojrhw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtdecnohnb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtceonvypk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtkiydzggz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigufen.top/gtaodwprtr.html

Ruby: File.size("a.txt")
来源：http://hz.zhoulong.xyz/gttqawzzqp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtivpqatab.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtkzpdhtea.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtmjpsnzil.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gtuyjkldec.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtfwxbwljp.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtzbrxpgae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtrndyhjjw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxinkj.top/gtqdfurwsh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtfvxkjotb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gturvmnxgs.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gthnyxegbt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtwpmitbfs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtsamygvec.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gthzrnkuov.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gttskngqdt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gtcuwppssz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtymcvqure.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtbbaaxpwx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtalixurru.html

[F12] CSV 读写
来源：http://hz.ppjwa.cn/gtkzdagwxp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtdbvfraor.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yanxiufei.cn/gtzegrupui.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gtkmqxxsvy.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtcgbruase.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtfmgwdwiv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtznzrcknv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhongyouzk.top/gtnblpesuw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtrryiifno.html

================================================================================
来源：http://hz.bjfxy.top/gtmtudhpas.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtannmaapc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtecadywsf.html

[G01] 定义类
来源：http://hz.yj20258888.top/gtkcjriyvd.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtnrqotrdq.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtnezabpia.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtmkawktpr.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtcqqtcxjk.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtydaklycj.html

Go:   type User struct { Name string }
来源：http://hz.sysykeji.top/gtvsilfxzb.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtdaoyecmi.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtnbuqffgq.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtvnpafqks.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gttouwrsnv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gtiormnsho.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtrptkhxei.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtefrbagfn.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtgwoclxhj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtbldjiaql.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.andypj.xyz/gtxmttcjkq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gthyfyvbmy.html

[G03] 实例属性
来源：http://hz.smart0.xyz/gtaqvqokvk.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtenehtkwx.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtiyvpejzn.html

JS:   this.name = "x";
来源：http://hz.sweek.top/gtsgqjempw.html

TS:   name: string = "x";
来源：http://hz.meibo888.top/gtzcjfzngl.html

Java: private String name;
来源：http://hz.smart0.xyz/gtxbuitaok.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gtibkvpyhn.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangtech.top/gtolyycyvi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gtopzomhat.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtszanjvti.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtfaqztnwl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtbolvcqfu.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtpojvvdrh.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtntbphnjd.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtdgyfsmgv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtlgqutrwv.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtlgpoknnu.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtbdpyvgqd.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtfiiwgvnx.html

Py:   class Admin(User): pass
来源：http://hz.ivvv.top/gtcgyndlmg.html

PHP:  class Admin extends User {}
来源：http://hz.zycfv.cn/gtoiuerjzd.html

JS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtqohfvjhb.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtscbrgxem.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtatsocyhg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtyknsmxip.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtgkgvhjtf.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtvcjlreme.html

[G06] 重写方法
来源：http://hz.xinyue.icu/gtpcozkyrk.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gthywryaup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtnkchczyn.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtryeenwog.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtiklakmhx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtoblqvnxr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gthnlppwav.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtzvamsxzm.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtjxwofctr.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtugrcctaf.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gtjlokagpw.html

PHP:  parent::greet();
来源：http://hz.jlsjyb.cn/gtgwodnxuu.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gthjpxelku.html

TS:   super.greet();
来源：http://hz.aizwys.cn/gtyvvwphrz.html

Java: super.greet();
来源：http://hz.tanke756.top/gtjiveytly.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtqwjmvvwu.html

Ruby: super
来源：http://hz.fzhhl.top/gtgbdsrkhr.html

C#:   base.Greet();
来源：http://hz.redwolf501.top/gtkvihgnlv.html

[G08] 静态方法与属性
来源：http://hz.shzxlz.cn/gtaipdozga.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtzcfkqdpm.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtqmhbmjkj.html

JS:   static f() {}
来源：http://hz.yuxming.cn/gtlwozdmhc.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtrexzfslp.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtzpvukcaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zycfv.cn/gtnrtudvrq.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtzarvgivy.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtymxilydf.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtlgblfjuf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydjk.org.cn/gtlcvdcdfm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shangyingyoupin.top/gtltxhdvnm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gthwlsoits.html

TS:   interface Shape { area(): number; }
来源：http://hz.kuanghao11.cn/gtydtvgefj.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtxgcotgng.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.316326.xyz/gtxxwiijqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtfotgxabn.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtzkoljdux.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtkilvkced.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangkeji.top/gtawuwhyhp.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gteyeywmka.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtbnauwqae.html

TS:   public / protected / private
来源：http://hz.vqdsnc.cn/gtfxgyugft.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gthmetlwym.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhixingplan.top/gtrucshynk.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtnstchddh.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtoyukdxpn.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gthlzcdzum.html

Py:   @property 与 @x.setter
来源：http://hz.gaohongyu789.top/gtgzriavzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtvpqblbsg.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtjmxwihqx.html

TS:   get name(): string { return this._name; }
来源：http://hz.yueranfly.top/gtmlsvvhjv.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtkwefbfwd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtgkrazrac.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangkeji.top/gtqlnufltv.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtcvqnegdu.html

[G12] 对象转字符串
来源：http://hz.9152youxi.cn/gtnvexkxna.html

Py:   def __str__(self): return self.name
来源：http://hz.jlsjyb.cn/gtunnifhsf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtqzdvtnqn.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtgbmobsri.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gttycubglt.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gthjbhaytp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gtorjbgdvm.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gthkemfaok.html

C#:   public override string ToString() => Name;
来源：http://hz.tian-w.cn/gtyuevweqi.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gtmwyclapl.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtjsgyjwjn.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtvuaxypbh.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtuyzrbylx.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtiesnafvq.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtsngjtgao.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtmxznfbpu.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigfzy.top/gtemnlhmtf.html

C#:   u is User
来源：http://hz.sxryk.cn/gtbwyvedjf.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtdwiefpxa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gtvrereppv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gttkbgtruu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtwznmuamg.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtfuxydkyi.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gthnnsmatl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gtzdiporsp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtgdgljtxh.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtkezolvon.html

[G15] 枚举
来源：http://hz.tian-w.cn/gttncdcfes.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtnhqiqxaj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gtaoxhbudn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yonumen.top/gtpjxpczwe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtwxwdhnol.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtmjweukye.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtvdnlwzmq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinyuanbaomall.cn/gtbimaooac.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtpscsfoch.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gtzlkeiiqy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gthpxstvky.html


<!-- 参考信息 -->