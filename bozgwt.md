代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtlldpsilg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.52xcode.cn/gtwslderwo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtmewlqtql.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtepllwnuq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenzaomai.com/gtmliwqlxx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gtsrwcnbbb.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtrtqaahql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hywenlv.cn/gtxovgmqur.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtdprquqkl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhiwuduotai.top/gtmjbcrqot.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sxryk.cn/gtxskcjcir.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gttwjmqknc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtvdoopvzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gtnltbpksl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtlrwtaazp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gthgznoenb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hywenlv.cn/gtmyqrshep.html

[E19] 多行文本按行拆分
来源：http://hz.yonumen.top/gtcdobwfvi.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtwpadvbbe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yueranfly.top/gtybltxrdz.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtbzqgjwou.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtrtgqhodr.html

Java: s.lines().toList()
来源：http://hz.xingfuxueyuan.xyz/gtcoavmisa.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtniujvtru.html

Ruby: s.lines
来源：http://hz.yj20258888.top/gtzjyjybgs.html

C#:   s.Split('\n')
来源：http://hz.cheryme.top/gtnndmrsuh.html

[E20] 判断字符串是否为空
来源：http://hz.yanxiufei.cn/gtwksgvwgr.html

Py:   if not s:
来源：http://hz.shangyingyoupin.top/gtrkpkfpcz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dianchejie.cn/gtlswfhvmf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtybcpgsdu.html

TS:   if (s === "") {}
来源：http://hz.wangshuangyany.cn/gtvfpsfgej.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtghjdpcdd.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtlpwrcyrd.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtnvlvblfm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtowchjetm.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtauoamtsa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xylfe.cn/gtbringeua.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtmxuomcfv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gthmnulkqw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtoyoqjemx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtmgqbyxdb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zycfv.cn/gtbryfpfsv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtbtytmxjx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.meibo888.top/gtmynzcsxi.html

[E22] 字节长度与字符长度
来源：http://hz.sufxvd.cn/gtdpdqgxsh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtmzeknosc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtxeuuopsb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtycwkiyld.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtwszpahhb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtxyextwcn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gttgvuidql.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gtkcxigyth.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtgfvjtwij.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkjgfnuzo.html

F. 文件与目录
来源：http://hz.fzhhl.top/gtaayaufus.html

================================================================================
来源：http://hz.meibo888.top/gtgtuhzfte.html

[F01] 读取整个文件
来源：http://hz.yj20258.top/gtchphtqzl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.snrcjt.cn/gtuuhxsxbw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtfaeqqizs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ivvv.top/gttyjrqwfj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtvkdijdzw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtrnokdbtn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gttvdabfux.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtwhcizxsk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ybcxt.top/gtvwbjloeg.html

[F02] 逐行读取文件
来源：http://hz.cucudq.cn/gthocobtth.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dashuyun.cn/gtualkhvad.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aizwys.cn/gtgyxvschq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gthbiftdyk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtaxfigdbz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtdykoeyrc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtplrwgsxx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hammf.cn/gtjhfojtkt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtscluejxv.html

[F03] 写入文件（覆盖）
来源：http://hz.ybcxt.top/gtlyibxqhh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtcjuxglbo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtxqaiibal.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gthnfkquox.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtltkssrtx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.haohaochexian.top/gtzybifgip.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cucudq.cn/gtkvyfowqu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dashuyun.cn/gtceihvccz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtklgkblbh.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtolbhqhma.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtybmrujgw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtjxzmksid.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtglhwgdkz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtgeqvgbqf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ybcxt.top/gtxuesfoqi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtjsgvhfzg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtszazkged.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtqqvdzbjt.html

[F05] 判断文件或目录是否存在
来源：http://hz.dianchejie.cn/gtkskdjhfs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj202588.top/gtiasplako.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gterynctvh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtoqajbnoz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtprfzocmc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtjiirvdxt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gthbpegbtr.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtjgtwfvgl.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtmxivnzta.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtuapevrgi.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtkppymfsd.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtbweekvcz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtxizngkgr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtvpsmygoc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtbccnvtfh.html

Go:   os.Remove("a.txt")
来源：http://hz.zhengqikj.top/gtxlhrvfyd.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtxztxetxh.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gtddljgllj.html

[F07] 创建目录（含多级）
来源：http://hz.tianlin.xyz/gtsfmhtsgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtoccjjydr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtvdsutuwe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtemfwepde.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtizxcapbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtgmlbxkmy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtngywtoam.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinghuilouyu.cn/gtofofeodq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gtxprntkjw.html

[F08] 遍历目录
来源：http://hz.52xcode.cn/gtpzxwflge.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtivxyuugn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fzhhl.top/gtkpptdyxb.html

JS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtgwgnggvz.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtvlvnqhxy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gttyptydjg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xinyue.icu/gtprvprldc.html

Ruby: Dir.children("dir")
来源：http://hz.ydjk.org.cn/gtzkvfrslw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtuuxfckgm.html

[F09] 获取文件大小
来源：http://hz.yj20258.top/gtmistkewq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtupwzmnvi.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtiwtgpmcf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtxryrgxbo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtcrnzlssh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gttedvkdwu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydjk.org.cn/gtuvgjmvcb.html

Ruby: File.size("a.txt")
来源：http://hz.sufxvd.cn/gtgfdvcxik.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenzaomai.com/gtszbbosdv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zycfv.cn/gtxruextcv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtpuykidbf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtaqkdomrp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtwjyzbgyy.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gtsqrjbqur.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtkdwrbrwr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtflkqknnc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbqcdoncv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cashguo.top/gtcuplsiik.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gteeyrgelw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtnvbompvl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtxkauyydi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtpioyugyw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtpwmhomno.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yanxiufei.cn/gtafiqpbpv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtcmgxnnca.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtcsyjmjih.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtunjcnwks.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtvadcqfwv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtsecusbow.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtkogsutqh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dianchejie.cn/gtkmojmrwo.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtmilmrjsb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xingfuxueyuan.xyz/gtnrinszxm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gtjrbqkuww.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtpgxkgbbq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtwyypfmyy.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvunqhqrr.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtghrjnpmx.html

================================================================================
来源：http://hz.guowangkeji.top/gtjammjbzd.html

[G01] 定义类
来源：http://hz.cashguo.top/gtbvwmgtjb.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtzwlpuvoj.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtasxzbtvt.html

JS:   class User {}
来源：http://hz.ybcxt.top/gthoxyeycv.html

TS:   class User { name: string = ""; }
来源：http://hz.quarkkingdee.top/gtrcfvhvdw.html

Java: class User {}
来源：http://hz.zycfv.cn/gtzgocpizd.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtgaryswbh.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtlmdezrua.html

C#:   class User {}
来源：http://hz.ivvv.top/gtchfoqbfj.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtepytljqe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtupzygpzd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtrudaaslc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gthehfarqz.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gtcsknaani.html

Java: User(String name) { this.name = name; }
来源：http://hz.sweek.top/gttbvwbrlg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtaxtqceel.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtizzpbjgw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtjukueuay.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtvpgcdbzo.html

Py:   self.name = "x"
来源：http://hz.gzhubu.top/gtiiecdlzq.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gtfxbhrxge.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtfzzipzno.html

TS:   name: string = "x";
来源：http://hz.yj20258888.top/gtcfpbthmy.html

Java: private String name;
来源：http://hz.quarkkingdee.top/gtayomaitd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guowangkeji.top/gtivskhuxm.html

Ruby: @name = "x"
来源：http://hz.tianlin.xyz/gtnnufymto.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.316326.xyz/gtwbhsadkv.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtvmldurln.html

Py:   def greet(self): return self.name
来源：http://hz.xinyue.icu/gtaqbnlmde.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtfdveqidt.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gtozbcetvz.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtfvryavbb.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gtuvtbhemr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtrmkblylp.html

Ruby: def greet; @name; end
来源：http://hz.daria6918.cn/gtkwfaineb.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtmmbyoknj.html

[G05] 继承
来源：http://hz.yj20258888.top/gtxxvcymbs.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtwhlgsjnp.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gttctudqtw.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtpobkrfpp.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtvinnohxy.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtmgfmdczv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gtryhzjkzj.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtcmrqjocf.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtcogpdxzz.html

[G06] 重写方法
来源：http://hz.jinqigfzy.top/gtglsmijis.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtrqdqzycm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gthqvoojpg.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtfystells.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtiyybvpjc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtdunoujvk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hysaishi.cn/gtpgfrbnac.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gthzklcovn.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtlrfhbgoi.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtwwmfirxj.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtmsqryyrz.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtyxgeiahr.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtservrpto.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gtdjqhbwgt.html

Java: super.greet();
来源：http://hz.tanke756.top/gtlclxhuli.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtdqbxwtrm.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gtriydrlmz.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gticcwvuog.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gtlkswqgso.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtbljqvpdc.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtalmuozxl.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtwrmgrwkm.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gttjfihchq.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtfqqitbei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gtaijsgxet.html

Ruby: def self.f; end
来源：http://hz.andypj.xyz/gtcivapxvj.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtfxrnuoiw.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtilnwjdfh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtbadewocf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sweek.top/gtitwlcuct.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gtdteixxni.html

TS:   interface Shape { area(): number; }
来源：http://hz.aizwys.cn/gtdupmqjsq.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gttzfahcdm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.havefunace.top/gtaijsazqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtwebzejmy.html

C#:   interface IShape { double Area(); }
来源：http://hz.quarkkingdee.top/gtcsjtpvyz.html

[G10] 访问控制
来源：http://hz.jianghu66.top/gtlpzmipbo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gtsczqsecj.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtsttqkfnk.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gtvtxrckzb.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtjkcfhokq.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtlefsaicb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtdcvmjhix.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtfixmxupv.html

C#:   public / protected / private / internal
来源：http://hz.jinqigfzy.top/gtyactzuah.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtopohuhkn.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtvecraeyv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtsnfnnjhp.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtisytsjnj.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigufen.top/gtvjugzobc.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gthtoiwdet.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtulobymhv.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtzlxvzkar.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtnwmsbbim.html

[G12] 对象转字符串
来源：http://hz.chenzaomai.com/gtewolbrki.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtrhozkdjs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtkvvehgkc.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtwwvmscch.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtcdsepyig.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gteenrbfff.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtsaikzpub.html

Ruby: def to_s; @name; end
来源：http://hz.zhengqikj.top/gtagmzjirf.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtrlyyckzo.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtxqxpucux.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtcytyzawt.html

PHP:  $u instanceof User
来源：http://hz.nanxinkj.top/gtdpjxywnn.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtdaubwiiw.html

TS:   u instanceof User
来源：http://hz.zhengqikj.top/gtzbzgnutt.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtmndrvqty.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtleamoxpv.html

Ruby: u.is_a?(User)
来源：http://hz.0kj1m.cn/gtofbilbyl.html

C#:   u is User
来源：http://hz.mhx1999.top/gtsjjgcwia.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gthmbwhlvb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.316326.xyz/gtgcicxlqi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigufen.top/gtnlbywnoh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtqnigxqxh.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtytfhtjvr.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtioxtucgz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gzhubu.top/gthjewflzm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtfxuvnypf.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtznmfxuih.html

[G15] 枚举
来源：http://hz.nanxuanxn.top/gtfgjabmuc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtkvpkvahv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gttumeszkg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtsrxyojxw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtqehhdthx.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtxelnkvbj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtrgzmjznx.html


<!-- 参考信息 -->