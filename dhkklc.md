代发 wailian999

Ruby: arr.tally
来源：http://hz.fengsongda.top/gtrttgvcnj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fzhhl.top/gtmwgiemcg.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtaixbzpce.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtihlwcvqb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtxluoufjy.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtqozdnxbt.html

TS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtzcfdggmz.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtflfunabs.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhoulong.xyz/gtwpjmprst.html

Ruby: arr.include?(x)
来源：http://hz.daxiang520.top/gtbpepazuh.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtfvwwinfc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aibaodan.cn/gtmazeckcf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.316326.xyz/gtqogfyets.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sweek.top/gtbvmgivdj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtfntkynar.html

TS:   [...arr];
来源：http://hz.nanxuanxn.top/gtjpserywb.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtrjlzhpyk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sxryk.cn/gtvtyspbuy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuanzhike.top/gtyrdqyzxq.html

C#:   new List<int>(list);
来源：http://hz.tanke756.top/gteatwaixw.html

[D23] reduce 累积计算
来源：http://hz.jyoumei.cn/gtsxzmmqow.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnqzz.top/gtwqrkthng.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cashguo.top/gtfaucisuh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtmznjyvlh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gtewicprrr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtenbiqsfm.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtehggquqd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yueranfly.top/gtfgdstrfx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yonumen.top/gtcppcberf.html

[D24] 字典 / Map 基本操作
来源：http://hz.xingfuxueyuan.xyz/gtzjnmgisy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gtvltjebiq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtdoizujwd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtsfhyxpaf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.9152youxi.cn/gtsepxdwuo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nwbrower.top/gtvzghdklc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hysaishi.cn/gtnhurpmsm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gtwuycmryh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gtwtfbypxv.html

[D25] Set 集合去重与交并差
来源：http://hz.vqdsnc.cn/gthrdqqvkf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gotoacloud.top/gtkwssumhm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhengqikj.top/gtltypvewd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gzhubu.top/gtkrzileqf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangtech.top/gtrwgdpdwa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gttbscptlk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtirljjafa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangshuangyany.cn/gtpvgvwwxj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.andypj.xyz/gtxfwmikxp.html

[D26] 数组转字符串
来源：http://hz.cashguo.top/gtjonstepj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinyuanbaomall.cn/gtylsenvoi.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtujcamrxg.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtbjbpmbju.html

TS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtgmgwgruc.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gtofspgalq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtlsmnbwsy.html

Ruby: arr.join(", ")
来源：http://hz.redwolf501.top/gtgpoyevja.html

C#:   string.Join(", ", list)
来源：http://hz.xinyue.icu/gtqgyirmpm.html

================================================================================
来源：http://hz.chenlongwang.top/gtitadfjsz.html

E. 字符串处理
来源：http://hz.nwbrower.top/gtwtmceaij.html

================================================================================
来源：http://hz.yongpay.top/gtioudwblo.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtbtwjfgaj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zdqjudy.top/gtbcsbhunh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hammf.cn/gtzzvnpsio.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtslnybrbr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtyitskyiz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nwbrower.top/gtekpgscnk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtlbfmiliq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenlongwang.top/gtvtwnckei.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtwiqudpwr.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtmmgtzcve.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtnhbxhbbw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj202588.top/gtqithnvqk.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtnapbvkwr.html

TS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtdxfdheas.html

Java: "ab".repeat(3)
来源：http://hz.fzhhl.top/gtvfnqlwnz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgfzy.top/gthbzrlphq.html

Ruby: "ab" * 3
来源：http://hz.kuanghao11.cn/gtyzurbzkk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtgokszsvu.html

[E03] 截取子串
来源：http://hz.zdqjudy.top/gtewouqscv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guowangkeji.top/gtyacmwwxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtqzpoaakb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtcigivefu.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtfuvfsjvn.html

Java: s.substring(1, 4)
来源：http://hz.cashguo.top/gtvovqghac.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtyexmnngs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gtilduuode.html

C#:   s.Substring(1, 3)
来源：http://hz.yuxming.cn/gtpolfyyoz.html

[E04] 查找子串位置
来源：http://hz.sxryk.cn/gtnewroxvc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhixingplan.top/gtfivoofzx.html

PHP:  strpos($s, "x");
来源：http://hz.redwolf501.top/gtgkuocpfn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gtlntvkjda.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtsidmczgh.html

Java: s.indexOf("x")
来源：http://hz.zhoulong.xyz/gtrxflaaod.html

Go:   strings.Index(s, "x")
来源：http://hz.yongpay.top/gtbvduuuon.html

Ruby: s.index("x")
来源：http://hz.ybcxt.top/gtluvebcqx.html

C#:   s.IndexOf("x")
来源：http://hz.tanke756.top/gttdxhizre.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gtzldpccqk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hongshengwenyu.top/gtssexatco.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtqvpmqook.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtljhszfap.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtnmtkycaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtnldlemkp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gtzmhkzmjd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gtrzbwpjfy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yueranfly.top/gtvajwtlge.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gtviplccnt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtyhohpcja.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ywan-chungtsiang.top/gtnrrcloys.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtlryhubao.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtxrfwrlgj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtkfwezzwt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtrldslbkj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yongpay.top/gtvchboscz.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtgrgmfywf.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gtfxmcbqqx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhoulong.xyz/gtladfyqef.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtubntegmv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gogol.net.cn/gtbtnexogt.html

TS:   s.split(",")
来源：http://hz.ivvv.top/gtahlkmusc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jiagoushi.top/gtrdnnzoaz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.quarkkingdee.top/gtvubhmsht.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gtpxcdsehp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtckuwlxok.html

[E08] 数组按分隔符合并
来源：http://hz.shzxlz.cn/gtmopkoztw.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtfmtmqwnu.html

PHP:  implode(",", $items);
来源：http://hz.zycfv.cn/gtznopfpbc.html

JS:   items.join(",")
来源：http://hz.52xcode.cn/gtuaskakgw.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gtnhwysytf.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtptraasqp.html

Go:   strings.Join(items, ",")
来源：http://hz.hongshengwenyu.top/gtwyjrszgb.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtfhklpoyn.html

C#:   string.Join(",", items)
来源：http://hz.feifeiyinyue.top/gtwckpkqrd.html

[E09] 去除所有空白字符
来源：http://hz.dianchejie.cn/gttzbxbfyk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtkobiigxy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.kuanghao11.cn/gtigdoasjt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gttgwaufoc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtjjespuqn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtnspuwmdu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nwbrower.top/gtsqbxbrap.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gtjbyydaec.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtctpxmfql.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cdnleiting.top/gtrokmmtjw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xziqi.cn/gteevcdrpe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gtqwewjwqy.html

JS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtxochsork.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtqzpxgqmo.html

Java: String.format("%03d", 7)
来源：http://hz.ivvv.top/gtjqjsvrsu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dianchejie.cn/gtmemrsecw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtjdtindou.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangkeji.top/gtgctzzuwd.html

[E11] 反转字符串
来源：http://hz.vqdsnc.cn/gtnebvhdca.html

Py:   s[::-1]
来源：http://hz.wangshuangyany.cn/gtnpwebtit.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtaluxqlzx.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtteqhclxf.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtxvndlaxy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gtsnruudpw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xinyue.icu/gtfobizemc.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtzuoxpyim.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtgkqnjgmo.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtzbxlejiv.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gttgvcvbzq.html

PHP:  substr_count($s, "a");
来源：http://hz.gotoacloud.top/gtqlpguuwu.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtmhamkzwz.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtazowlgow.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hysaishi.cn/gtosqwlala.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtswsydzqy.html

Ruby: s.count("a")
来源：http://hz.sxryk.cn/gtdokkuhld.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtjmcvnxdb.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtoiwjabvo.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtlafzboxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hywenlv.cn/gtunqlpozh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gttqmreyyh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtrkgztopn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.snrcjt.cn/gtfnglovsq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtppxrspfj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.haohaochexian.top/gtnemodzgr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtysxpkipy.html

[E14] URL 编码与 Base64
来源：http://hz.dianchejie.cn/gteymtkdwf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gthwpkjjah.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtwlhbumkd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuanzx.com/gtiknjdeve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shuidangran.top/gtluekdgzx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258.top/gtzkirxdvg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtxjwwtxaz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuetiantiany.cn/gtpkypbygf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydjk.org.cn/gtyiwejpbm.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuanzx.com/gtmbupevpr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtlodwheey.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258888.top/gtykiptlql.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gtumvynhbp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sufxvd.cn/gtgkzkjryi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ppjwa.cn/gteoxbpvme.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtlmfhefdi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj202588.top/gtxxiijkgr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xingfuxueyuan.xyz/gtpzzhwsit.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtoqfhwkqx.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtbrqirnuo.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtyzntbwcl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtfkhcjjpw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtjdvwpqat.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.0kj1m.cn/gtzdjfftie.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.316326.xyz/gtezxcnzjx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gtiekyxhmp.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtgchvozyw.html

[E17] 首字母大写
来源：http://hz.hammf.cn/gtlmwvhmdo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sufxvd.cn/gtzlbvmuky.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtrjxzfmib.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtpmipffbp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtcvypmpep.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gtvnkmcxia.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hfpthk.cn/gtloqrmylb.html

Ruby: s.capitalize
来源：http://hz.aizwys.cn/gtktryaszk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtdzclespd.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtourxklbj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtmlcfzwko.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtpxamprpq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtpnxidier.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtbxnobvsr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhongyouzk.top/gtubhfdloq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gttzzyxuys.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gzhubu.top/gtmyntlyqf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigfzy.top/gttxaieunf.html

[E19] 多行文本按行拆分
来源：http://hz.cqqwz.cn/gtkcdqepte.html

Py:   s.splitlines()
来源：http://hz.yangfankeji.com/gtykwtizzt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtnpmvwnzs.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtiuogmyfe.html

TS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtfsmgvwin.html

Java: s.lines().toList()
来源：http://hz.yj20258.top/gtijjdhdqj.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gthycxoftv.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtvrzwpzpp.html

C#:   s.Split('\n')
来源：http://hz.tian-w.cn/gtxxfvjxdk.html

[E20] 判断字符串是否为空
来源：http://hz.chenzaomai.com/gtyewjbyub.html

Py:   if not s:
来源：http://hz.dianchejie.cn/gtuptmxlzt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtrudrefzs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gzhubu.top/gtsfqceime.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtnlrprkml.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtglhrnacn.html

Go:   if s == "" {}
来源：http://hz.ydjk.org.cn/gtqtqzvyzq.html

Ruby: if s.empty?
来源：http://hz.hysaishi.cn/gtjyrixbag.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gteqpfiqgu.html

[E21] 超长截断加省略号
来源：http://hz.yvedp.cn/gtjxfmgwrs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtudelsodc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtjjyqtnep.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtphngjrrw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtjxoyjuox.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtmggjeoit.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtszjksrre.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtpnovmsoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtgoxxvgqu.html

[E22] 字节长度与字符长度
来源：http://hz.birdmap.top/gtetlsbyru.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aibaodan.cn/gtgtudshcy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtiplqsgjj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtyutizfni.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtphjhlcmn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtpafizmkw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gtssvmwvvf.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtcihcgivl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.smart0.xyz/gtpgvkytrf.html

================================================================================
来源：http://hz.cashguo.top/gtgrsgjnra.html

F. 文件与目录
来源：http://hz.ybcxt.top/gtqvtftjcz.html

================================================================================
来源：http://hz.ppjwa.cn/gtuxqymijs.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtussbgidt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gtujvtygxa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtzblxxavw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtovchunpx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtdxcjapgq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gttplcbdes.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gtxxuuizbx.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtnnuezfrh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shuidangran.top/gtyvvrbsdv.html

[F02] 逐行读取文件
来源：http://hz.cucudq.cn/gtdywbuciw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangdashe.top/gtiofklzer.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hywenlv.cn/gtfmwhpyjd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtdaqcvxor.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtwjqigwba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtvfrnmwaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xinyue.icu/gtsjrkhdal.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xuetiantiany.cn/gtgveunctk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtdrcvlgjb.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtndrqzaru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guannengcc.top/gtzvvhlmqy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtgrjikyby.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gttwmydkru.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtopffdtfv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtulsxqcmc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yangfankeji.com/gtpowkhynx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtineydrdc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pycfn.com/gtcaiigiab.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtkrtdzptr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinyuanbaomall.cn/gtddcmdtje.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtbzhghszr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtsxhkphls.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtwzmymybo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.c1oappe.top/gtqvvvtkow.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangdashe.top/gtpqzezmcc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zdqjudy.top/gtpybhdhjj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtwwsmjyjs.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhongyouzk.top/gtpovpiryi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gtayscovuy.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtpxkvdskf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtchhbacfv.html


<!-- 参考信息 -->