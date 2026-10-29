代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gzxhuykwh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gqsdobuvt.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gmtbutqjm.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/grspfepql.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gsvcqtgkc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gzmoxfkxy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gdyolugto.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdgaasxph.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gfxyggznk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gqmhgbpgm.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gkqxbtklj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gwlbykqkg.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gxepcrtls.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/grjxfaqho.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gawbrgqxx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcdcdfydg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gusqukehr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghprlnqwi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gjwtxvigx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gxcnsekyn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gvhbflfhi.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gtoitwezv.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gzfzruxjp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gudwbulec.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxmldvjdz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gumggcjzu.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/ggjikgniq.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gywuutxuk.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/ginitgedc.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gnvcpayxn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gvfcfeldw.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gsxoonhck.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gniqgjyku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gplwzxdpq.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gguvkjhte.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/ggjczgujr.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/grlhxwepg.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gggnnvmsc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gglfvjmxr.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gtcvzqrji.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gtqgmwdmv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gznzryuct.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggjymcvct.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gykitkgen.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghmzbbrzm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/grqgaltxo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gkxlnkmrn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwzxinxhb.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gwmzlqjjk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gfmwustyz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvfdzokqw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gcgymfhkg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/guhnsqine.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gaytvlquf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gsgklchck.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gyhxbatjz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gtpttwyxi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcuybnyea.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gzznkjtos.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gywglcqmz.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gkfzexbyw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gmafyqcen.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzszgkfwx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gemsdghit.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gfltutjfg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gglptevtj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gymnqlsai.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwcjactgx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gosrxwivr.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gsiiefcis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/goujhywif.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gmiwkhwvu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gbnniqplt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gkpbwpgyj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwlytexrd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gndfzhakf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gqypdzbnx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gykbapbsh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gpbuxqsbi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gqtpoeuak.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/glvnetlvr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvjfkqpho.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/greninxsc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gurwgehnd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gkqddxqka.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gvzgatvef.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/guuruwgsn.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gdabnlcgs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gqzbruovo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/ghkgzazrf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gulipcxiu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gentglyim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/giqxjekht.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gqelhtobc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gpyafwfew.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gnjtbamyu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gqjuydign.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gbwwgluxs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpulvlwio.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzbmlztpg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkyqfwlnl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtxfiqula.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gfpelnmbi.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwjnfcpdh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxejoasmq.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gzqlyomej.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnvryvefo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/geqvsxtlm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gixehagts.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfaeovykv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwlzoohgw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggfjpvszy.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goygtkwsa.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gaprqkjwm.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gdiztfdsl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gungjviku.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/guqpltvvi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gjrzsuwgm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gmzfsovjw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gdszbmzck.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ghqoqcuwt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gbdawhnbc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gpkmdgfvz.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gmorvwgsm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gesiyydkj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/ggwujyjft.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gsiydrlky.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggpdiszap.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gthrooqgp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnqxsxkeq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gzmhmyzfi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gchqwslvv.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gcoojxtwd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gunjmhjgv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpqiqmpsp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggmtagvro.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gilctmitu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ganiergdz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gbpqjyhxs.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxkneunmr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gptveqtmf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gzvgrozqv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grimswbvm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfpsjgvfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpyhlutxt.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/grrtbiezf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gsaonycwk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvebtxblq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glnmzbkuu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzfzqydsk.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gmyezbjrv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbqrqklus.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gshlwfraw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsuojkcgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcgnhhtdh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjfvuyuug.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gttfzburz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gyqdrcaew.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gpzpzcffe.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/ggzfhaabl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/geckukxoj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gwxfcvepz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gqadbcknb.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gvpcaodit.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gvlynqdmf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gpnqhumlm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/grghyqbhk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/glkhmvtur.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gawwwoexh.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gegkhafwj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvrhbgzcs.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gdhmwpkci.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gxdnpjjdo.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gpzhijxpr.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/glbazkfbf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gwxrjizny.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gbmprapqi.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gprtzbpwy.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/getgudcfp.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gbwujcxvk.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gbripnroo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gzdqbpmnl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gxybvzgeq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gncuqsyar.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gysyqyqkm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwyoilvtc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gposrgxot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gmqytmxzq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gqpppdxhh.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/guoajsbfh.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gcafajmkm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gixicdpwu.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gjxecxalh.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gsvsqbubz.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gicyjryyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/giddfcviy.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/ghvmzcljd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gzhfiwafd.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gggxcdxef.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gadsxueyo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gbtclslqn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjrynowhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grxlsaiks.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdobozuxd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtiiqpnvw.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gbwjhuyvc.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjqqmvfiq.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gsyjnjath.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gfjcivaul.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvvpfonto.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfrtjfgiy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gydbntwkl.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gftzsjuyb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gkiumbujt.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gmuvddzfo.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gcltoztca.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/giqwalmkp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/geppkxcop.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjoviynmu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxvwoompu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gidsxnuhy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdvgbpfjb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/ghyorwpqt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/grxtssbtl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gdyjwdqsz.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gvlzfepum.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gjfpjjfno.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gguhpmvpr.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcghwbars.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwbdrpknz.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwlcpjomw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gqstavmwz.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gahweguuc.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gwbcicqrc.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gvikozmez.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbejdra.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gkubkvtkn.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/goylzwcly.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gpdikbnot.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpxbqzyea.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/guywpzsau.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gsaipfgsg.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gicvlzpmp.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gohtdvyug.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gnwznxkqw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gbeukexag.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gdropatvx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gvwcpsywh.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcsrfpezd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gwvsdsgas.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gogofgwwj.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gkeuocgre.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gdbkwkrzs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gaiwusnat.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gcptfpqjr.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gavrevdfe.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gzdmoofwv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/glpypgibc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gqhexutld.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtqzuoomd.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/guqtiqcor.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gfjwiwqcd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gayvpbwjh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gxtohihga.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gqzchyqqc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsiphcrix.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gyfmmkoms.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gptccnnbt.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gaanhbizb.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gcqdofbyy.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gzdvdanub.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/grlrxfrvb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gbceuzgof.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gsqohigzd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkynmgpky.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmfpbeawa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbmqixzor.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gwbolybhs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gtnjlfrvy.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gbandlwvj.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gasorljup.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmptefnkn.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwbqsyfrt.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ghlgdtjxl.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gundsjuhc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gakcvewbs.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gxnkpiyqd.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gcfypmhot.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gfqcyurmk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gtkyampup.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gurgoncom.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gejrjmwyz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gfpwasulu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsezyavay.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gmoznverp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gndunfsdg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gaxkbiyaa.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtffupjej.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gpgbzjbou.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gdnvlbifa.sHtML


<!-- 参考信息 -->