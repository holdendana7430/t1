代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtsyzpbwta.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtljksjbtb.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtjscvbbxe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtxnmxldfr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgufenzy.top/gtnhhlxmjm.html

[D24] 字典 / Map 基本操作
来源：http://hz.pycfn.com/gtzjxfccrg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangkeji.top/gtwvtetvdv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtmanewolg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gaohongyu789.top/gtmijcmpcl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ivvv.top/gtuhntnslz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtcvpeitxx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtrszppftc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hfpthk.cn/gtzokuxzum.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhongyouzk.top/gttadmnllp.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtxalqthgr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tian-w.cn/gtfmacssrt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xinyue.icu/gtavjgault.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gaohongyu789.top/gtkzezaohd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangtech.top/gtjhpbfrzj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zycfv.cn/gtpgoptgts.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtdrfahwbu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtvwfsuxpg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cheryme.top/gtxrrrrown.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtinaecsky.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhijiandao.cn/gtbkslzlth.html

PHP:  implode(", ", $arr);
来源：http://hz.zhixingplan.top/gtbtcdvajt.html

JS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtetetdemy.html

TS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtdbdydbwn.html

Java: String.join(", ", list)
来源：http://hz.tanke756.top/gtpzigabuh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yonumen.top/gtxgymynrm.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtaqzhvzps.html

C#:   string.Join(", ", list)
来源：http://hz.quarkkingdee.top/gtzptkndxg.html

================================================================================
来源：http://hz.daria6918.cn/gtwxfvnpte.html

E. 字符串处理
来源：http://hz.yanxiufei.cn/gtaclzpkbd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfrfbunhu.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtnunxduvc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtmgtjhnaj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xinyue.icu/gtcraliske.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtaryjbvrv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gteflpywtw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtlkynozwi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aizwys.cn/gtjxkffqpe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gtdbxrmakb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtvhpxsljq.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtvfrgdlzb.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtzfjkfles.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tanke756.top/gttfvbuanr.html

JS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtlbteisik.html

TS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtjqiqsdex.html

Java: "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtbmgjuykg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtimjsmopp.html

Ruby: "ab" * 3
来源：http://hz.hfpthk.cn/gtyqqkzias.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtbcpptzpo.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gttmcwkasj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xziqi.cn/gtxefelyok.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gtoyrfymbg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gttozncdrc.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtswncfxfc.html

Java: s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtetwabzux.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cdnleiting.top/gtoalzrnie.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtbdmiudyh.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtqbzvbauh.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtccxowrlh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jlsjyb.cn/gtdznbvwva.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtpogrehde.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinyuanbaomall.cn/gtjjlboblr.html

TS:   s.indexOf("x")
来源：http://hz.hnqzz.top/gtjpkxclyi.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gtvaelolkh.html

Go:   strings.Index(s, "x")
来源：http://hz.ydjk.org.cn/gtxrvsafce.html

Ruby: s.index("x")
来源：http://hz.sxryk.cn/gtmlcxlcmp.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtgvtrhgby.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zycfv.cn/gtinbonxvz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xziqi.cn/gtoedmwann.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gaohongyu789.top/gtoaqxriso.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtbcypzomj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.316326.xyz/gthdhtcrsk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gteejewela.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenlongwang.top/gttxsdewak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtgwqrwvir.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gtsjyqgfhu.html

[E06] 替换子串
来源：http://hz.ehwqpu.com/gtljtaothw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtlesjtqkq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jyoumei.cn/gtukjopkzc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtqgolpybu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtrkszcans.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtcscyuubj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtjbepqgxr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nwbrower.top/gtctrvjszi.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtascmlivv.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gtphslvfew.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuanzx.com/gtxydtywwx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nwbrower.top/gtuepaflip.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtjvmbcqhw.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtmlkiesyz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtsbmumzjv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xziqi.cn/gtcjbstube.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gtzgcyuzkq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtuafzlkbg.html

[E08] 数组按分隔符合并
来源：http://hz.ybcxt.top/gtngbfeorw.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gtkfrvqpjf.html

PHP:  implode(",", $items);
来源：http://hz.chenjidiqi.icu/gtjizryhkl.html

JS:   items.join(",")
来源：http://hz.yj202588.top/gtuprlnika.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtclhjznyj.html

Java: String.join(",", items)
来源：http://hz.yonumen.top/gttnnifild.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtagsafwnf.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtabvsuype.html

C#:   string.Join(",", items)
来源：http://hz.hnqzz.top/gtzpnscpkm.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtnrcuyfcv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gtnsohazjd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daria6918.cn/gtjspznhds.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtpbrxewyp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtyydjyipe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtvcclswcd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gtqimmfivo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtunwoulpl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yongpay.top/gtzskequdd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgfzy.top/gttjqjoyyv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtgwajdmsw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtxpcqajxv.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtfxjdviev.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtazqbgjpi.html

Java: String.format("%03d", 7)
来源：http://hz.birdmap.top/gtbvkbtcok.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zycfv.cn/gtmfvuigdb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dashuyun.cn/gtzmaxdeoa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ydzc1.top/gtviofvssk.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gttcheriyh.html

Py:   s[::-1]
来源：http://hz.zdqjudy.top/gtozelvjkr.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtiyngetyp.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gttgxodehe.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gttovaobwt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.vqdsnc.cn/gtazvblcts.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gteakwehvc.html

Ruby: s.reverse
来源：http://hz.fengsongda.top/gtumssbbyx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtnjeyskmu.html

[E12] 统计某字符出现次数
来源：http://hz.tian-w.cn/gtsmpfrthg.html

Py:   s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtzzvooxji.html

PHP:  substr_count($s, "a");
来源：http://hz.316326.xyz/gtzifuwrqm.html

JS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gttcuvccya.html

TS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtuuguiicp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtufcitexr.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtumakeaav.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtmpvxiqav.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gtqegsqpyv.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtpbtdflrn.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtzfjnjidr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtjmmuhgvo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gtmisgywja.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtlcwecdlh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigfzy.top/gteegwlpej.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hongshengwenyu.top/gtsvomvqmo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtbaqfazny.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yonumen.top/gtjexbhxha.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtgqpnthkc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tianlin.xyz/gtqdnpkvjo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tianlin.xyz/gtwdrmgpia.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtgtwqmzko.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhengqikj.top/gtuzklapkr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtwalccrhh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gttygmcgji.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtyhotikft.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangdashe.top/gtzzckvgyn.html

[E15] HTML 转义 / 反转义
来源：http://hz.fengsongda.top/gthqaskoiz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtlmhmejgh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtvmtmvlur.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daxiang520.top/gtjxmruhhv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtzhpgbhig.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtxbjjifiz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtdvzalfbs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtqmrmtzla.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtcbsdmxbg.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtwustytgk.html

Py:   f"{1234567:,}"
来源：http://hz.jiagoushi.top/gtmzlscrda.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtcwxkbpxi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtjomeovhy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtrqcutnxd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtlkjwteka.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hysaishi.cn/gtoxyoyxkc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtxknjsdld.html

C#:   1234567.ToString("N0")
来源：http://hz.shangyingyoupin.top/gteygvmixy.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gthpcjhdsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtqimdhyrr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gttigyvdxc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtlqtelcty.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtrbskpbse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxinkj.top/gtrrnbpmzr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenzaomai.com/gtlkwgpijf.html

Ruby: s.capitalize
来源：http://hz.tianlin.xyz/gtafpwgqvm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtmsajwlms.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtvatyuwdy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtkbiolsnd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ywan-chungtsiang.top/gtlcykdivv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gthgwihrxn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtpqjyatfo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hysaishi.cn/gtfrxmnvkx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtkdgbikbi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cdnleiting.top/gtgejnobqj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.feifeiyinyue.top/gtaqkajzry.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtzexpkwue.html

Py:   s.splitlines()
来源：http://hz.nwbrower.top/gtvzpmvjrl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gtxlzpxtte.html

JS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtxcwegumw.html

TS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtenfahksc.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gttdtvrpxj.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gtwbirqjzp.html

Ruby: s.lines
来源：http://hz.chenjidiqi.icu/gtlfcsoexj.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtkuhhxvti.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtgfteknex.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtyzcccvea.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtiqjmvapn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtqsvgbndq.html

TS:   if (s === "") {}
来源：http://hz.ivvv.top/gteddjbxzj.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtalmhucry.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtxzneragi.html

Ruby: if s.empty?
来源：http://hz.wangshuangyany.cn/gtnqdznowl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtuqkzcxpc.html

[E21] 超长截断加省略号
来源：http://hz.zhoulong.xyz/gtrfvzqzpr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtwpkbxoyo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtzqxrtlye.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtfzltbfmj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtkvwpcjpv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtojdeffgu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtrfxooyct.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtshzdguzp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtjzxeijcl.html

[E22] 字节长度与字符长度
来源：http://hz.hfpthk.cn/gtryelxezy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daria6918.cn/gtktolpkua.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtluzsgyvf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtfxlduieu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtqmyrbbge.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aibaodan.cn/gtjvwakzzh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gttghikajl.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtsyfyiorr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gttkzydlrw.html

================================================================================
来源：http://hz.havefunace.top/gteatlezun.html

F. 文件与目录
来源：http://hz.yj20258888.top/gtkhqvbapf.html

================================================================================
来源：http://hz.sufxvd.cn/gtqdqwpvuo.html

[F01] 读取整个文件
来源：http://hz.svipenyu.cn/gtfbirmusr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gaohongyu789.top/gthhhjggwy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.birdmap.top/gtjhabbbfz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gttlzvdqfr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtxetomonc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtmxxsqqzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gtgxgascyw.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtcbxfdynh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtphmeggwu.html

[F02] 逐行读取文件
来源：http://hz.yj202588.top/gtnsrtfvot.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hysaishi.cn/gtabaggnzj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.52xcode.cn/gtovigtdxu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtwyccwcvj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtfeetfcpq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtgmtzykee.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shangyingyoupin.top/gtbcichctu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guannengcc.top/gtjgofkkby.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenjidiqi.icu/gttdshxefm.html

[F03] 写入文件（覆盖）
来源：http://hz.nanxinkj.top/gtrtlczcdb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtjiuonhzm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtmygbhlzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtfddhtasw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtddkaqkwv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtcvkdxpqn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtwmlpqhgn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydjk.org.cn/gtyehtdiup.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtpjfoqwyk.html

[F04] 追加写入文件
来源：http://hz.hnqzz.top/gtsnonnhmf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daria6918.cn/gtzloqephm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cqqwz.cn/gtllopmaio.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtjadtjeuy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtaxhonitn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gtodgetogt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtxvojihhp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtjqqjghfl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gotoacloud.top/gtukevhlck.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangshuangyany.cn/gtjhldsdtj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtfmbnstqz.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtwcddfkpi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtilxuwtwt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtiuyacfut.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtscstxkhb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hfpthk.cn/gtibpxblot.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtpaxroyrg.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtwddamzou.html

[F06] 删除文件
来源：http://hz.fzhhl.top/gtazwqnrue.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtlqutatmc.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtopqblfjs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtxyqajwkm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gthhbobmrf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtpvvtlnnw.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtakcwcgxr.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtqfuniful.html

C#:   File.Delete("a.txt");
来源：http://hz.dashuyun.cn/gtccwskvoj.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtpvqpfqww.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258888.top/gtxrdlkafw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtwhopuigv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtryxlutpa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtgwmnmdat.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hammf.cn/gtxeygtdpz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtqcodiefj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtxkskitdx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtoyuumwlu.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtqhryqamp.html


<!-- 参考信息 -->