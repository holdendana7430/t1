代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.birdmap.top/gtiydyuzpr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigfzy.top/gttxjbakdu.html

C#:   1234567.ToString("N0")
来源：http://hz.xziqi.cn/gtmexydpvc.html

[E17] 首字母大写
来源：http://hz.chenjidiqi.icu/gtrwctamvg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtdzzvynpr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtaepiwimb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtpictbzpo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtiiaawnwq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.mhx1999.top/gtkgudzbfs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.kuanghao11.cn/gtgxnlftob.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtszcsnmac.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.quarkkingdee.top/gtfiwsnweh.html

[E18] 模板占位符替换
来源：http://hz.aizwys.cn/gtuhoqsfzo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuxming.cn/gtyyxvzivp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jianghu66.top/gtntulvdnk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtaorjskww.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtreprpfwg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sweek.top/gtsuarjyho.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtnuaygmzv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gtqzbgwzov.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtrbgpfbaq.html

[E19] 多行文本按行拆分
来源：http://hz.shangyingyoupin.top/gtaxmgeapw.html

Py:   s.splitlines()
来源：http://hz.ppjwa.cn/gtdijtmakv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pycfn.com/gtvxexwhgq.html

JS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtiypzmauz.html

TS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtqqabeujl.html

Java: s.lines().toList()
来源：http://hz.zhoulong.xyz/gtbkiyzohk.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gteftubrhd.html

Ruby: s.lines
来源：http://hz.birdmap.top/gttxctvpsw.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtprwljsts.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtkvgjzhdj.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtqjfhacvx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtfuturtwo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.redwolf501.top/gtydcvhpxb.html

TS:   if (s === "") {}
来源：http://hz.jqgfzy.top/gtxnklgcha.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gttnoypkad.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtwypbqxkz.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtkskzxbov.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.9152youxi.cn/gthoptrtfm.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gthmhwxghu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.haohaochexian.top/gtcwcvryko.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtkpvqtsjv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtrjkmaqye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtknlzdrfx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtmgwdniwd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtmhnyfhte.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.andypj.xyz/gtmzrpwnnq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cashguo.top/gthbfklbns.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtvdnhnprh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtfemhmdxz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtyjshmkfa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtnclrfjln.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtujpkwdoy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtszfxrpro.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtpwuaniqr.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhiwuduotai.top/gtqfyextan.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtahwmqshp.html

================================================================================
来源：http://hz.chenlongwang.top/gtaphziupt.html

F. 文件与目录
来源：http://hz.jinghuilouyu.cn/gtomsflfol.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdtlpuvsn.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtboterzpt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtxvdsjenr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtzsqomhbu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sxryk.cn/gtqgzxmsha.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258888.top/gthmxspinh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtxhrnnkez.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cdnleiting.top/gtogmzeymh.html

Ruby: File.read("a.txt")
来源：http://hz.0kj1m.cn/gtrpuusybk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cheryme.top/gtubfoqxoh.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtssbqqsgk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yanxiufei.cn/gtysvhhqhb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtksbbpifh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gthifyidue.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gttkbxtyeq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gterbpjjif.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtgxssuaek.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtrpyfxubz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hfpthk.cn/gtbiwhzcpo.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtrwyxwjru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.quarkkingdee.top/gtykiyjgzt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtvlxfmcbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtfkgmbfnn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtqzlvcmtc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gttjufaqdk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gtpnhmogle.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.9152youxi.cn/gtmssjycpq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtohozzkxh.html

[F04] 追加写入文件
来源：http://hz.aizwys.cn/gtozcyxrxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtwqpzikar.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xziqi.cn/gtewqyiadi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtufkxzxmr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtymelgmdz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtdiuzlsas.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gttoxgzneu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ppjwa.cn/gtlpswvdlg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtdxtxgfvd.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gtmcldberm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jyoumei.cn/gtsvvfgghb.html

PHP:  file_exists("a.txt");
来源：http://hz.aibaodan.cn/gtbmueluha.html

JS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtxkqbqlke.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtxcziffjb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtyfembewr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj202588.top/gthszpimpq.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gttlbzdqjh.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtfxhctgdw.html

[F06] 删除文件
来源：http://hz.c1oappe.top/gtvyedtasb.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtmifvlgwr.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtwkmmeodj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtkmpttgiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gttkytxqvu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtahrpbole.html

Go:   os.Remove("a.txt")
来源：http://hz.cqqwz.cn/gtzlgibhlk.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gttcbwaxiv.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtwpenyybu.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtgruixhgh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtavhppxxy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jianghu66.top/gtpamtdgiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtwbnhsxae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtjbyuupar.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gtsutejkfw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtgrpniliz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cdnleiting.top/gtxudxdpab.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gaohongyu789.top/gtmaykknzz.html

[F08] 遍历目录
来源：http://hz.hysaishi.cn/gtodurcafy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.quarkkingdee.top/gtmmmawgoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtrfkepzxk.html

JS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtxjcfzegj.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtsiqsjdgn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtpemjyixd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtxcxnypxb.html

Ruby: Dir.children("dir")
来源：http://hz.zhijiandao.cn/gtryfybogy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtpxscpweq.html

[F09] 获取文件大小
来源：http://hz.iojbl.cn/gtgsflkfuv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gtduzbgzyv.html

PHP:  filesize("a.txt");
来源：http://hz.jyoumei.cn/gtnuvgdxli.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtygydxzkf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtxlpviedn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtxfjpitgz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtyytjuerd.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtrptrqmrr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtsxmislgt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtmyxaunzl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtmpjnstoj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtupylocav.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtxyvudsit.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtzexzbvrb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jyoumei.cn/gthmihrrpc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnqzz.top/gtirkapwyr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gthvdxciui.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtfzeofcql.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtvcrdwwxv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtdbqudyfk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtljmcxpsz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtddajpmuc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtrmujiszs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnqzz.top/gtomxjgpup.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.9152youxi.cn/gtfjrrfwyv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtoljrsscj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtsofgvgpy.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtvgvhtjum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtahcguhoz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtvhsbnquv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.andypj.xyz/gtnsrppiqx.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtatdorxtv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhixingplan.top/gtiywweabg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtlanqyqvf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gteofurwro.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtezbprdvi.html

================================================================================
来源：http://hz.sweek.top/gtmgjolpzx.html

G. 面向对象
来源：http://hz.zycfv.cn/gtphmxmupr.html

================================================================================
来源：http://hz.cucudq.cn/gtjdtbxwtx.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtihmwmbam.html

Py:   class User: pass
来源：http://hz.xuanzx.com/gtqcfxaksa.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtexvcjzkq.html

JS:   class User {}
来源：http://hz.hysaishi.cn/gtrttwfgdj.html

TS:   class User { name: string = ""; }
来源：http://hz.ydzc1.top/gtiywbzlly.html

Java: class User {}
来源：http://hz.fzhhl.top/gtcyctbikw.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtemgqxowa.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtnbfmoqyz.html

C#:   class User {}
来源：http://hz.birdmap.top/gtmylqdyar.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtsbfqwaik.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangshuangyany.cn/gtaudiyjqh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtrlxmiizd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtjwvfzpny.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtltqylswc.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtwekxireh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ppjwa.cn/gtiuxikmnv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtlihcerzd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangshuangyany.cn/gtxkutegsp.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtigmrxkoy.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtusmikbkz.html

PHP:  public string $name = "x";
来源：http://hz.zhixingplan.top/gthmtpryeg.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtmdcemqnz.html

TS:   name: string = "x";
来源：http://hz.yonumen.top/gtncqrcxwv.html

Java: private String name;
来源：http://hz.gaohongyu789.top/gtsoygambj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gthwzdivik.html

Ruby: @name = "x"
来源：http://hz.pycfn.com/gtkaxtchra.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nwbrower.top/gtyskpcepe.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtcggwuski.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtihibusuo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtpbtmzdpy.html

JS:   greet() { return this.name; }
来源：http://hz.dashuyun.cn/gtpmjkvazl.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtfpxvqnlk.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gtvxtfsxoq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258.top/gtnpikuxyn.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtsxznlfdi.html

C#:   public string Greet() => Name;
来源：http://hz.dashuyun.cn/gtkhffaebu.html

[G05] 继承
来源：http://hz.tanke756.top/gtvyyofjqr.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtygacmtgc.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtdgmwjkrt.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtgkokawmn.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtjxoeankh.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtbyecxmwj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtvfrncjrp.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtjjksxzgo.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtixndfuii.html

[G06] 重写方法
来源：http://hz.havefunace.top/gthqxgruct.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtznooefmg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtdmqvynjc.html

JS:   greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtiihbliyc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtzcwoilfr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtsulgxspl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtqmiuyrgg.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gtcdpkoiya.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtfuzmzalo.html

[G07] 调用父类方法
来源：http://hz.nanxuanxn.top/gtcepgwhrw.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtfhzfxsgi.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtasmobsvs.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gtqqwxtxlh.html

TS:   super.greet();
来源：http://hz.havefunace.top/gtqhysfwux.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtjzzhiuhx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtedcdbrzc.html

Ruby: super
来源：http://hz.hfpthk.cn/gtlzhprtcj.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtyloeyiru.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtyuckwzgw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtpznkahym.html

PHP:  public static function f() {}
来源：http://hz.hnxiangtu.top/gtgancpnby.html

JS:   static f() {}
来源：http://hz.zhijiandao.cn/gtqnemxvsg.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gtsawlplzo.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtntbujxdv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtidvhcdmn.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangtech.top/gtggbzlaaq.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtlqfogmqm.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtdgxbcifx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nwbrower.top/gtkivixxty.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtjuapmhfm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhongyouzk.top/gtsnxbwaif.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtdcmblvws.html

Java: interface Shape { double area(); }
来源：http://hz.quarkkingdee.top/gtagewlaak.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gtaymnhuoh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtppiptefz.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtwyrppzhc.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gtbvlafpam.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zycfv.cn/gtshjkukon.html

PHP:  public / protected / private
来源：http://hz.xinyue.icu/gtfmlneyrj.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtabiyfauh.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtlxbcuize.html

Java: public / protected / private / 默认包级
来源：http://hz.cucudq.cn/gtenbqewpl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtbprulbkk.html

Ruby: public / protected / private
来源：http://hz.zhengqikj.top/gtoqrztcxz.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gthdektfnd.html

[G11] getter / setter
来源：http://hz.quarkkingdee.top/gtjyhhmxtg.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtonpemeuv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtacdelpgd.html

JS:   get name() { return this._name; }
来源：http://hz.wangdashe.top/gtcrkohjfq.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtzickssyv.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtypoateic.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtszaxowyp.html

Ruby: attr_accessor :name
来源：http://hz.tian-w.cn/gtoheinrci.html

C#:   public string Name { get; set; }
来源：http://hz.svipenyu.cn/gtveknbngr.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtpjcsucgj.html

Py:   def __str__(self): return self.name
来源：http://hz.redwolf501.top/gtoksqmgar.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtwfgmjopr.html

JS:   toString() { return this.name; }
来源：http://hz.c1oappe.top/gtysnygeqe.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtngjkzcde.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gtpnixmuzz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtcowcirgo.html

Ruby: def to_s; @name; end
来源：http://hz.gzhubu.top/gtgcmpxkfe.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gttvzjibbz.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtmaprenzo.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gtmfhybqjo.html

PHP:  $u instanceof User
来源：http://hz.shuidangran.top/gtbbkixglh.html

JS:   u instanceof User
来源：http://hz.ehwqpu.com/gtxuisiysz.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtzvhfqkyr.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtpvpjcwre.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aizwys.cn/gtgyvhgysz.html

Ruby: u.is_a?(User)
来源：http://hz.hammf.cn/gttrjwmvnb.html

C#:   u is User
来源：http://hz.guannengcc.top/gtiwjdzoyh.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtmjvvdghu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtbyzcjbpg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtgumblywn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtsyhajfkn.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtlvnrntri.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtljlgxvpa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtodljffhg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yvedp.cn/gturqgpsuf.html

C#:   record User(string Name, int Age);
来源：http://hz.0kj1m.cn/gtdptgbknk.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtpfuahcbo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtuqqxnxne.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtoklttkek.html


<!-- 参考信息 -->