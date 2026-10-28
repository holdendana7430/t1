代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.xylfe.cn/gtwtvebten.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gttfwtpuwe.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtoseddqap.html

Java: list.contains(x)
来源：http://hz.hnxiangtu.top/gtgidwifqj.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhixingplan.top/gtuzcvzoxz.html

Ruby: arr.include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtzycryowp.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtltwrmnzy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jqgfzy.top/gttqoohrgd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtabsnhyek.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gtcqwjeegf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtkikthwtm.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtnuwrdeax.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gtzsedwvho.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtkqdqhouj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtmcotibcd.html

C#:   new List<int>(list);
来源：http://hz.pengpengdd.cyou/gtyzbcexyh.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gtzytaqnma.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guannengcc.top/gtmfmzgayi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gtldsligoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtxcnqfufp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtgnzcznge.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yonumen.top/gtodldjyec.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtenwiixbw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cqqwz.cn/gttawqclnc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtxilzsmzh.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtcqdhpezv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtangckybw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.iojbl.cn/gtddvqujtl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenjidiqi.icu/gtfyptazfp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hywenlv.cn/gtshiteycb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tian-w.cn/gtztbqxzwc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pengpengdd.cyou/gtebksjwwb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtoncxdfer.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cdnleiting.top/gtnnnohiyl.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gthdjgxyvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigfzy.top/gtnkkaivlh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zycfv.cn/gttthkcmlg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtdrnhvxva.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jyoumei.cn/gtvmcnvtwo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuetiantiany.cn/gtssigstcy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shzxlz.cn/gtqbqtmlux.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.birdmap.top/gtzwbkrljm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydjk.org.cn/gtdevqzcjg.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtrtbstmwb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtxkxqxzrc.html

PHP:  implode(", ", $arr);
来源：http://hz.zhoulong.xyz/gtcjcojfgg.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtimnieqbh.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtqntdiulb.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gthebltcff.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jlsjyb.cn/gtiifhqwgu.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtrszwxhig.html

C#:   string.Join(", ", list)
来源：http://hz.yangfankeji.com/gtcvfqchzg.html

================================================================================
来源：http://hz.yvedp.cn/gtipqmzfpc.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtldpsvyrj.html

================================================================================
来源：http://hz.havefunace.top/gtyvlrbcaq.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtavcywedx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangdashe.top/gtgtvhmgyb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daria6918.cn/gtcccvgkxc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtnngvruaa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtqrvvpebw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jlsjyb.cn/gtihsoszli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jiagoushi.top/gtybkeclwu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtjcqaghru.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gtdybbgedi.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtiaxminrp.html

Py:   "ab" * 3
来源：http://hz.nanxinkj.top/gtisjknimu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gaohongyu789.top/gtxtrztkhd.html

JS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtpkdiigch.html

TS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtfbwecvdd.html

Java: "ab".repeat(3)
来源：http://hz.yangfankeji.com/gthxqhyvis.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtkvljkhqi.html

Ruby: "ab" * 3
来源：http://hz.yongpay.top/gtdurtuvxy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fengsongda.top/gtyhutvxgg.html

[E03] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtbgjaivcv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhijiandao.cn/gtwvyiinwn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtuihpdeot.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtznkpzvdv.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigfzy.top/gtlrextojl.html

Java: s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtolgkrong.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtjeydzmep.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xziqi.cn/gtbooktzcx.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtcvhqirzp.html

[E04] 查找子串位置
来源：http://hz.jianghu66.top/gtqvafcyqe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.guowangkeji.top/gtlotpgrxz.html

PHP:  strpos($s, "x");
来源：http://hz.ehwqpu.com/gtoamxmcfb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuetiantiany.cn/gtfyhikoqo.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtmnwyivlg.html

Java: s.indexOf("x")
来源：http://hz.xziqi.cn/gtbprhfvbj.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtyejgsdnp.html

Ruby: s.index("x")
来源：http://hz.sysykeji.top/gtlhdgzjqx.html

C#:   s.IndexOf("x")
来源：http://hz.yanxiufei.cn/gtbkghagso.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sweek.top/gtikjqqrdb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.haohaochexian.top/gtxuclwvov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pengpengdd.cyou/gtonkzorfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtizxkxafq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yanxiufei.cn/gteownlqbz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtsnezhxyf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangdashe.top/gtphhlbzhc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtxjufuewf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtyxpwuayh.html

[E06] 替换子串
来源：http://hz.svipenyu.cn/gtfleqqitn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dianchejie.cn/gtltezjgkp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangdashe.top/gtwmgrqykh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtaxntckzs.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gthaxfqkfa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtykxvjowu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hysaishi.cn/gtsadmnhud.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhoulong.xyz/gtdwplkscj.html

C#:   s.Replace("a", "b")
来源：http://hz.sxryk.cn/gtunjougzo.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtcrxzguuv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtznocotjv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtvpehduhd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ybcxt.top/gtjtutbbyx.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gthnkastrq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gtjdmcfhuw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtfmxjldrp.html

Ruby: s.split(",");  s.split
来源：http://hz.yanxiufei.cn/gtykoxmcme.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhoulong.xyz/gtssxcrprn.html

[E08] 数组按分隔符合并
来源：http://hz.zhiwuduotai.top/gtvbftkcfy.html

Py:   ",".join(items)
来源：http://hz.kuanghao11.cn/gttqrvrsuq.html

PHP:  implode(",", $items);
来源：http://hz.yangfankeji.com/gtoqpuduux.html

JS:   items.join(",")
来源：http://hz.guowangkeji.top/gtjccsdjnt.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtszjvskux.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gtdkphutlv.html

Go:   strings.Join(items, ",")
来源：http://hz.fzhhl.top/gtvtxmlwdf.html

Ruby: items.join(",")
来源：http://hz.zhongyouzk.top/gtenbqkcuy.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtzheewjcn.html

[E09] 去除所有空白字符
来源：http://hz.mhx1999.top/gtcfaczpfe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhoulong.xyz/gtnvastjze.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhijiandao.cn/gtkqozqjvw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gttiaytcpn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtfcoqxcez.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zdqjudy.top/gtltqkcxvc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangdashe.top/gtubsyzajr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.mhx1999.top/gtepxusfcn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gotoacloud.top/gtvvifnkke.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sweek.top/gtfivnkpmk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yvedp.cn/gtbpgbbyix.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gtbfsvquun.html

JS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtrjjsvmyl.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtypcofebo.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtqmntmxfi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gogol.net.cn/gtwlnvnuio.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtfyeghjpd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gtumnfpubs.html

[E11] 反转字符串
来源：http://hz.tianlin.xyz/gtuvapezlj.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtshblpwol.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtzfteuanj.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtquchtitk.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtzzlermbp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtlziboceg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.quarkkingdee.top/gtaihncrih.html

Ruby: s.reverse
来源：http://hz.tanke756.top/gtwktqzevh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtcqdjngpr.html

[E12] 统计某字符出现次数
来源：http://hz.yangfankeji.com/gtkxoitloz.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtfjenpbmb.html

PHP:  substr_count($s, "a");
来源：http://hz.mhx1999.top/gtczwskdqf.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtrphmxdek.html

TS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtciicspcj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.haohaochexian.top/gtrguccpoi.html

Go:   strings.Count(s, "a")
来源：http://hz.0kj1m.cn/gturkazuoc.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtvyqnfoav.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuetiantiany.cn/gtixkmofia.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtujmenxyi.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtssyrdnfk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.feifeiyinyue.top/gtxxazfhtt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtfvckmlgg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtquxhkdxf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtpuszzujj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aizwys.cn/gticpauoat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shangyingyoupin.top/gtpmrespgt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtwvqburne.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gttixqmlnh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.c1oappe.top/gtnhhgpmcc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.kuanghao11.cn/gtqoltiiph.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinghuilouyu.cn/gthyznwghf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xinyue.icu/gtwdvhrqwg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xinyue.icu/gtcortznjn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtneolyrhc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnqzz.top/gtoxyttxoe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtampzrynj.html

[E15] HTML 转义 / 反转义
来源：http://hz.kuanghao11.cn/gtkiuohnvc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtlzgdeayn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtfsenbczb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dashuyun.cn/gtksnzzfgb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtpkwpvidb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ppjwa.cn/gtkkegrrtc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.feifeiyinyue.top/gtnabkuefy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtmeyoyfjl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gogol.net.cn/gtrustlygk.html

[E16] 数字千分位
来源：http://hz.daria6918.cn/gtqobmapno.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtepoyoawo.html

PHP:  number_format(1234567);
来源：http://hz.hfpthk.cn/gtznwchewx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gthdqofgzz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gthtltengt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtgluvpoar.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtfqmkgwcv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtkcwrlszf.html

C#:   1234567.ToString("N0")
来源：http://hz.hysaishi.cn/gtuaqcegov.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtkiyembja.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtlklslzek.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtxvhlocxo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtzddfcyjy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtzzlslxcq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtgwdhdtyn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigufen.top/gtmbctmeqj.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtvloinbbn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtbxybqvmw.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtyqktlqso.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ivvv.top/gthcfqjsue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gtlktigmdu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtvjtqjlno.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtlffvzhxs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yanxiufei.cn/gtcoyvylye.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtkfgjybuo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinyuanbaomall.cn/gtifnyrhbm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtnlylftki.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gteuplsgjd.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtcdydksns.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gtbovvqbxg.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtbelhuroy.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtzkwkqynz.html

Java: s.lines().toList()
来源：http://hz.redwolf501.top/gtcvgkywyw.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtssprnocr.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtimtpnalk.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gturbukewx.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtauiovxtl.html

Py:   if not s:
来源：http://hz.zhiwuduotai.top/gtiyqlsjfw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtsgcvlnss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtizxhehuy.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gtbxnnjakf.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtobqjimsc.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtdawbiluu.html

Ruby: if s.empty?
来源：http://hz.daria6918.cn/gtnblxdsbd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtbaokcbkp.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtmtheimtz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cdnleiting.top/gtiqkrfcnv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtgtvinxgx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtnirjhrrb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtwihwlrxc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gthiwdlryw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigfzy.top/gtvxydvpqn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zdqjudy.top/gtftjygbif.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtpswzftxi.html

[E22] 字节长度与字符长度
来源：http://hz.yangfankeji.com/gtuwqtjzwg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtphugkxui.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gttigidvju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtvryymdvq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtbxjcfpil.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtgccjjndf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hongshengwenyu.top/gteokfnnlq.html

Ruby: s.bytesize;  s.length
来源：http://hz.ywan-chungtsiang.top/gtbislzobr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtgxhzcokl.html

================================================================================
来源：http://hz.bjfxy.top/gtyojurccl.html

F. 文件与目录
来源：http://hz.jinqigufen.top/gthoixytda.html

================================================================================
来源：http://hz.tian-w.cn/gtjhfcdktu.html

[F01] 读取整个文件
来源：http://hz.sysykeji.top/gtanxuhsbp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtfbyhsxsg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gzhubu.top/gtmijhwhbl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtabgxpkvd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj202588.top/gtgiteylwn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gttcljbxjc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.svipenyu.cn/gtusyuqenl.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtappdxfyg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shzxlz.cn/gtwafjuvny.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gtpadaokvd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.mhx1999.top/gtitmfuuso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxinkj.top/gthoihackn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtcgrcwmqb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtmswwigjr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtzokxvnii.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gtlvrmcpof.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangshuangyany.cn/gtpaptmtyr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258.top/gtpnhjyrxj.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtcvktizbk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.iojbl.cn/gthccxalmj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtvmhfgerp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtyaewfcpq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtktvrhgxp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtrjhxcccg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yonumen.top/gtkoovznlp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hfpthk.cn/gtoluboufc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shuidangran.top/gtwngyfgbf.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtftljacnj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtsqtkuptz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj202588.top/gtpcfjlmkg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtikyrupmx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtrqwjkcbv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gtjxyqazsi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.haohaochexian.top/gtdygqodqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shangyingyoupin.top/gtvgtojddj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtwckwkybl.html

[F05] 判断文件或目录是否存在
来源：http://hz.sufxvd.cn/gtfntimwjg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtcrdxehpg.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtwzpbsytj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtbcqebzuu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtqjekuvqb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtcjwltmow.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenlongwang.top/gtpavvxqle.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gtlxhmuwfa.html


<!-- 参考信息 -->