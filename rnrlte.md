代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.daxiang520.top/gtamqecwrk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dashuyun.cn/gtmsdethkl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gttcnjnwhk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtdetrpujc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtgbqlmmne.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtpkrfnyum.html

Ruby: s.capitalize
来源：http://hz.aibaodan.cn/gtfzlyzdcy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtbahfvsdj.html

[E18] 模板占位符替换
来源：http://hz.quarkkingdee.top/gttcijalzd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gtcsuzdckv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgfzy.top/gtwcqkbcma.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtszgvuyar.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtfcwhkbgm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtmscocakv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.vqdsnc.cn/gtbmkqvojs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ivvv.top/gtelajbkdy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtpwspryjo.html

[E19] 多行文本按行拆分
来源：http://hz.sxryk.cn/gtqtkfvszh.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtpvnhqhtg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuanzx.com/gtlgdjkewg.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtwuzpwcyr.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtpcvfysrs.html

Java: s.lines().toList()
来源：http://hz.sxryk.cn/gtbtvvhryk.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtojfinelo.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtokpzavqs.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtqvuabcws.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtwjmsvvtf.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtmdipioxa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258.top/gtotijmivd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuanzx.com/gtpmfemzly.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gthfujrnzx.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtjczacbye.html

Go:   if s == "" {}
来源：http://hz.sweek.top/gtyhveimvj.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gtjmkwxvvv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtvbnbmnsp.html

[E21] 超长截断加省略号
来源：http://hz.gogol.net.cn/gtuevpskwr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtmnxduqqi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtsnirkmwb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtyazlgyrg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtrqfxfitg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtgtejlwsp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtqdsnoaef.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.andypj.xyz/gtyljeupku.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtueudxxbi.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gtmvgnyjez.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenlongwang.top/gtaadcuvei.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtvtywbxww.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtknehhork.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtqzfxtvje.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtxmxreyzp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gtfqxapmsk.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtetlrurhd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtvbqtbjyk.html

================================================================================
来源：http://hz.316326.xyz/gtiqucxpjh.html

F. 文件与目录
来源：http://hz.ppjwa.cn/gtaqtrbwdj.html

================================================================================
来源：http://hz.pycfn.com/gtilwxpvvf.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtbfzfqauo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtdtqymvjk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ehwqpu.com/gtkoquulta.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtpdonupyu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cashguo.top/gtgpgrljie.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtouimvinr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtznljiidx.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtqqerghdw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sufxvd.cn/gtjwofvgxf.html

[F02] 逐行读取文件
来源：http://hz.cheryme.top/gtdaxeeyrw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gtdgwkrrki.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtgdxorahp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtjljraxki.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtdegfaimd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtothxxzdz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtniknqfha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tian-w.cn/gtuevjvtxw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuanzhike.top/gtkmdvvced.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gttlcmeduu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtaergzdvr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtpznerxbf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtodumzyiw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gthlbvejoz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gtfnnkvwxe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtspbvjoss.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtkkcxidyt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtropjzxyr.html

[F04] 追加写入文件
来源：http://hz.tianlin.xyz/gtqddtvbar.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pengpengdd.cyou/gtvnrqleke.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtnqpsgogg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtiounxkte.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtsaypbxwb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtklxrdlfi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtwwrasgql.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhixingplan.top/gtoakllcrv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtazteqoet.html

[F05] 判断文件或目录是否存在
来源：http://hz.guowangkeji.top/gtsmuelgle.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tanke756.top/gtptgwtpwo.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gtghfdkaqz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtskukbetq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtmcsslxbb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtelmxrjhs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtuuobdnfi.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtswvrjwgh.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258.top/gtwytlztft.html

[F06] 删除文件
来源：http://hz.jqgfzy.top/gtabrghtea.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtnkvxipag.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtylokxatd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtvjpicoyn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gtpzmwymzf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtjrdirhlj.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtzuzwigfa.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtyoiwenns.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtehdqsubb.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtxqlbjfic.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtocqehkkx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtzomlrjdo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtcgryjdhs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtxkreoxzh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtmessddbx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtvzfftcgp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.snrcjt.cn/gtushphprt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj202588.top/gtuocrbevs.html

[F08] 遍历目录
来源：http://hz.chenlongwang.top/gtipbcbmyv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtqkclljsr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtaqrhfipo.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtxuxdxyel.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtjlgfkdzc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtuasfhseg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtfxafbukh.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtqngcaywg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtxaflknsz.html

[F09] 获取文件大小
来源：http://hz.daria6918.cn/gtkdqdguzg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gtbiubxpia.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtnvibskoo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtbflfzqqk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtwjsihhdi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtizgbhfir.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtpqobwqhu.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gtpozajakf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.meibo888.top/gtjfwoybzj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtbfrsqpmx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtqcxgwbew.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtvkfhxzsz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtwhdljgbp.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gttahyxius.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtirayocst.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shuidangran.top/gtphukpmtm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtsvwsogde.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtrhcnxsoz.html

[F11] 复制与移动文件
来源：http://hz.zhongyouzk.top/gtfadwxnws.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtlqlcgzyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtqwlgwhpa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtjwmtexcr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtlnqvdzbk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.pycfn.com/gtnqkoisxi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtbnxuzyzc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtowebotdm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtegywljft.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtxcpfmduu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtvfzxbiyn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtcwxfzsit.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtmkdvpyyu.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtfsgmmukx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hongshengwenyu.top/gtpqxplfwj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtctpltlso.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gtfborkcik.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ybcxt.top/gtossdudbu.html

================================================================================
来源：http://hz.cucudq.cn/gtnuduidwp.html

G. 面向对象
来源：http://hz.yongpay.top/gtwstogjre.html

================================================================================
来源：http://hz.cdnleiting.top/gtdjiqxyrn.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtmiifpmdx.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtwxurvamg.html

PHP:  class User {}
来源：http://hz.redwolf501.top/gtauzfcnci.html

JS:   class User {}
来源：http://hz.cdnleiting.top/gtduyeqpyu.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtqikzcvhb.html

Java: class User {}
来源：http://hz.yuanzhike.top/gthflkwhmp.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtyhtmnvfj.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtryczvhii.html

C#:   class User {}
来源：http://hz.wangdashe.top/gtaukekbwu.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gtwfpzlxtl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtblyzmulh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jianghu66.top/gtjnsupbta.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtshzwjhcc.html

TS:   constructor(public name: string) {}
来源：http://hz.xinyue.icu/gtfudqgjby.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtjumdnzhz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtofuobwic.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cqqwz.cn/gtdwtorbbu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtwfroexdp.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gttjrfivrk.html

Py:   self.name = "x"
来源：http://hz.jyoumei.cn/gtqqtnvlae.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gtuqsfolsp.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtkewgtzty.html

TS:   name: string = "x";
来源：http://hz.sweek.top/gtrtuqyqnr.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtpftfvgzr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtrdusjqmv.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtokctqqyt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gttaftkdic.html

[G04] 定义方法
来源：http://hz.jinqigfzy.top/gtncyiwqxl.html

Py:   def greet(self): return self.name
来源：http://hz.gaohongyu789.top/gtotbzcbdh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtapwpfnrm.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtyigqbdbk.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtxukqidfr.html

Java: String greet() { return name; }
来源：http://hz.zdqjudy.top/gtqydrahgc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gttgxrcdiu.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtcyohyxyg.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtxgkycamr.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtsivvclmh.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gtluriawre.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtxzkdopfx.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtknzcyfzz.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtspyyodld.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gteflxnupr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gtxgjnhqdu.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtbuguhvnv.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtydywizrd.html

[G06] 重写方法
来源：http://hz.yonumen.top/gthafnwqyb.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtmznamifi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtukkdoagw.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtjkjceuna.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtjvgzeiif.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtsuydidqg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigfzy.top/gtkeibamkm.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtypsjvqpl.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtgnumtpwi.html

[G07] 调用父类方法
来源：http://hz.yj20258.top/gtpcqjxufl.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtrtazghat.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gtsdburndt.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gttmgxuczh.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtkhmtxoqx.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtasvxtkjn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.svipenyu.cn/gtbhxlxdoc.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtbsmrdbnf.html

C#:   base.Greet();
来源：http://hz.ppjwa.cn/gtzzeicswr.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtgqdorcje.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtzpapwljk.html

PHP:  public static function f() {}
来源：http://hz.0kj1m.cn/gtjavatuco.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtdwsnpdti.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gttethmyal.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtfofnibzk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtzsywjfaq.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gttannpuzb.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtktrbjqlo.html

[G09] 接口 / 抽象类
来源：http://hz.tanke756.top/gtbvnaszfw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtoibitlow.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtuvyiegta.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhoulong.xyz/gtqmjlgjaa.html

TS:   interface Shape { area(): number; }
来源：http://hz.yongpay.top/gthiwjpizb.html

Java: interface Shape { double area(); }
来源：http://hz.redwolf501.top/gtiobpuabo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtfxthiunb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuanzx.com/gtymtfxhcr.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtrxmfgflz.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtsoxulrzo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ybcxt.top/gtfarkhetl.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gttgfpxokx.html

JS:   #private 字段；其余公开
来源：http://hz.zhijiandao.cn/gtwymmoxmj.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtslzgrqlk.html

Java: public / protected / private / 默认包级
来源：http://hz.daxiang520.top/gtapeqvjbm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jiagoushi.top/gtrupgppvf.html

Ruby: public / protected / private
来源：http://hz.jlsjyb.cn/gtjkvdywuy.html

C#:   public / protected / private / internal
来源：http://hz.snrcjt.cn/gtfdymuzcl.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtsevarmpd.html

Py:   @property 与 @x.setter
来源：http://hz.xuetiantiany.cn/gtvzkxsjkl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtfjxwqamx.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigufen.top/gtlvkqonby.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtbxcxvres.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtjplonhcz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtsvujncud.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtnrmmcymy.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gtjcvunbna.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gticjrpqoh.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gtkhmagubc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtteezmxgc.html

JS:   toString() { return this.name; }
来源：http://hz.smart0.xyz/gtiqqffbdo.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtghsuberi.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtqnnslefj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.smart0.xyz/gtvjljyxlh.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangtech.top/gtqijqpxgr.html

C#:   public override string ToString() => Name;
来源：http://hz.chenzaomai.com/gttpucynsa.html

[G13] 判断对象类型
来源：http://hz.hnxiangtu.top/gtgsndnweb.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtgvlpvhkd.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtrgqihnxi.html

JS:   u instanceof User
来源：http://hz.havefunace.top/gtezcwisbz.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gtjskczvpn.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtkepmxddq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtfuwcoxyb.html

Ruby: u.is_a?(User)
来源：http://hz.ybcxt.top/gtmfgsaqpx.html

C#:   u is User
来源：http://hz.shuidangran.top/gtzwfnojwt.html

[G14] 数据类 / record
来源：http://hz.hammf.cn/gtwfsnhqas.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtrgfjlida.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ybcxt.top/gtdrwsgxmg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.52xcode.cn/gttspbtyij.html

TS:   type User = { name: string; age: number };
来源：http://hz.feifeiyinyue.top/gtptaorfme.html

Java: record User(String name, int age) {}
来源：http://hz.jianghu66.top/gtcrvnzndp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtprkcknge.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtrbumkwdz.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtzukokbwa.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtjphhhxoq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zdqjudy.top/gtjlacfzhr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gttbsqrhql.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ivvv.top/gthmvqsamx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtjzajanzm.html

Java: enum Color { RED, GREEN }
来源：http://hz.sufxvd.cn/gtzikqmvcq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtgzsngkqk.html


<!-- 参考信息 -->