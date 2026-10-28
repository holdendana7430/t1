代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnxiangtu.top/gtsgpfisnq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtdxzqdkxx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gterodbidl.html

Go:   // 手写 map[T]int
来源：http://hz.hysaishi.cn/gtrdcartus.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtwfnslmkk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yvedp.cn/gtmcxfhbyz.html

[D21] 判断是否包含某元素
来源：http://hz.pengpengdd.cyou/gttvkkrgax.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gttfoksjlx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtxquzbtqo.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtmsdcxfnp.html

TS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtjhyrreqw.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gteacrebks.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtpjzmhzqe.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtbziiobac.html

C#:   list.Contains(x)
来源：http://hz.nanxuanxn.top/gtkbtkaowx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtzqfrqyzu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtixnvfysb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xinyue.icu/gttqbkdyzd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtkaknkvnd.html

TS:   [...arr];
来源：http://hz.daxiang520.top/gtopgcouqb.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtfevqauhg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydzc1.top/gtopmwnzbf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtxlwdehjk.html

C#:   new List<int>(list);
来源：http://hz.fengsongda.top/gtaclvzbql.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtvsqpvxsn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangkeji.top/gtggkodfbp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.mhx1999.top/gtgbgrqwwh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gthnkkuwro.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtpfdabxmr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gticirwnou.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtinpxqvwm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxinkj.top/gtpzavmkvk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinghuilouyu.cn/gtcdbxbfox.html

[D24] 字典 / Map 基本操作
来源：http://hz.meibo888.top/gtwyrnmmso.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.bjfxy.top/gtpvszcwny.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtmrshwsrx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.feifeiyinyue.top/gtcfjfgodi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gaohongyu789.top/gttvjicgsv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gthfueilyh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ybcxt.top/gtxepevbyu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtlofpimbg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cqqwz.cn/gtgbzjfdfl.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258888.top/gtxykgdtxm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.redwolf501.top/gtospkfggx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yvedp.cn/gtarcktowz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gteasdljez.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.meibo888.top/gtoqayllqf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtlommmnsk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtgtbddgat.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhaomingkeji.xyz/gttffpffxf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fzhhl.top/gtwztqxpqn.html

[D26] 数组转字符串
来源：http://hz.haohaochexian.top/gtpleqdafr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.0kj1m.cn/gtklnhpvfv.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gtunczinao.html

JS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtfjtrzeuf.html

TS:   arr.join(", ")
来源：http://hz.cheryme.top/gtxfwmbqqr.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtfulkwfdd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gtxbgybuwd.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtcpaldmgf.html

C#:   string.Join(", ", list)
来源：http://hz.yvedp.cn/gtrugiobeq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtngzwfcju.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtsfzfxzqv.html

================================================================================
来源：http://hz.yongpay.top/gtgumvyugc.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtsyjgyhtg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtdbixxbgc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtptgafajw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gthqveolnd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtexewogaf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gtifxuodxr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtakjznpdx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtxhrizlxj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtxdftaqbz.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtfgyhvloo.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtuzspqxiy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.svipenyu.cn/gtahdulfbk.html

JS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtwvjbgpza.html

TS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtfuqxgxmr.html

Java: "ab".repeat(3)
来源：http://hz.fzhhl.top/gtwuahfcvs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangkeji.top/gtvqwyftue.html

Ruby: "ab" * 3
来源：http://hz.zhiwuduotai.top/gtmniqnagc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtfrrjjwgl.html

[E03] 截取子串
来源：http://hz.zhoulong.xyz/gttzrwnxjs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dashuyun.cn/gtshgldchi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sufxvd.cn/gtibkrvump.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sysykeji.top/gtnzzkyhpb.html

TS:   s.slice(1, 4)
来源：http://hz.cucudq.cn/gtdruhsunk.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtamacqsqw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtpvakorgt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtqzgkdgsa.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtfuphwlmk.html

[E04] 查找子串位置
来源：http://hz.cqqwz.cn/gtonniwjhr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xylfe.cn/gtpzeosbyj.html

PHP:  strpos($s, "x");
来源：http://hz.pengpengdd.cyou/gterltnzxu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gtnosnwtzh.html

TS:   s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtzwrbwzcp.html

Java: s.indexOf("x")
来源：http://hz.jianghu66.top/gtqbyhsdal.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtudvstlsz.html

Ruby: s.index("x")
来源：http://hz.ybcxt.top/gthhjbocat.html

C#:   s.IndexOf("x")
来源：http://hz.chenlongwang.top/gtaxdoiiik.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnxiangtu.top/gtxyrkcptn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.mhx1999.top/gtrewzuwfl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gttfgwasfj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtlgjpnnib.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtflnvhsaj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtktmrnmuu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinghuilouyu.cn/gtrmodddnd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gttzrhpvzl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hywenlv.cn/gtqufggojw.html

[E06] 替换子串
来源：http://hz.jinghuilouyu.cn/gtadgzhsga.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtvjqhkomo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenjidiqi.icu/gtfqnxwvqg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gteokihyfc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtsuewzoxd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtrrlrkdig.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtnjhwagvo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gtegkxtics.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtaivpvwoi.html

[E07] 按分隔符拆分
来源：http://hz.sufxvd.cn/gtiuwkrlxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258888.top/gteznnwdwu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtwmrccliv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fengsongda.top/gtzuzytgbi.html

TS:   s.split(",")
来源：http://hz.gotoacloud.top/gtuykevyjd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtmxyehsoq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yongpay.top/gtrtxmebsw.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtedijhjtg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258.top/gtugughhfi.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtdgjukdpw.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtqkhqgejb.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtlupkucqb.html

JS:   items.join(",")
来源：http://hz.nanxinkj.top/gtfwtxkbjt.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtrzhpphqz.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtyfxfglwo.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gtlmmbihsr.html

Ruby: items.join(",")
来源：http://hz.hfpthk.cn/gtbyzwlxjk.html

C#:   string.Join(",", items)
来源：http://hz.pycfn.com/gtrnzfguci.html

[E09] 去除所有空白字符
来源：http://hz.aibaodan.cn/gtdlfwieyf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hysaishi.cn/gttrjloaav.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.kuanghao11.cn/gtqandywkt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtdswjcmhu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gttucuqzsb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuxming.cn/gtfxpjbtsk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtvyvmlqze.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.svipenyu.cn/gtoisjjjtf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhoulong.xyz/gtzwksxsax.html

[E10] 左侧补零 / 定长填充
来源：http://hz.mhx1999.top/gthxawjhdu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtfzooqnjo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fzhhl.top/gtdlxjizxw.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtqebpbrtg.html

TS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtshtqykid.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtlxmgvitd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dashuyun.cn/gtojpktzxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gthrpqhdqq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gtbebgiegz.html

[E11] 反转字符串
来源：http://hz.iojbl.cn/gtpvgdabrz.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtkvwwobxn.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gtzivohllh.html

JS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtgtesqqvr.html

TS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtyjqcewlh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxinkj.top/gtmdhfrbiw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.bjfxy.top/gtyfsyvfde.html

Ruby: s.reverse
来源：http://hz.yuanzhike.top/gtyqmbroud.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtvwdbgopl.html

[E12] 统计某字符出现次数
来源：http://hz.hammf.cn/gtdoiqifpn.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtbygzouvy.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtuyslurwu.html

JS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtqflbfsjj.html

TS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtlxegdcpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtrgdwlnad.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gtvwdfrmeu.html

Ruby: s.count("a")
来源：http://hz.cdnleiting.top/gtonfnmeyb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhongyouzk.top/gtnqeszsqb.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtanpjiwej.html

Py:   for ch in s: print(ch)
来源：http://hz.aibaodan.cn/gtwymfhoei.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gtkucdakdv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtylzzexpo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtddienemw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtrotvawwx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtdplqkfdy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ybcxt.top/gtcsvzlkhu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtdgjxlglm.html

[E14] URL 编码与 Base64
来源：http://hz.xuetiantiany.cn/gtlsonzuwm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtxhizmlsf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yonumen.top/gtzutjljxu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jianghu66.top/gtchfeyato.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtnhytcyoc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangshuangyany.cn/gtvvttwnpy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinyuanbaomall.cn/gtpjztrjno.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gogol.net.cn/gtfjgkjfkg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtdwaoyghi.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinghuilouyu.cn/gtgfmbahnm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gteijkmidb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtgqjvnwgp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuetiantiany.cn/gthdaejsjq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtzwvtquxe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtflaigdrz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shuidangran.top/gtvqkhpqnk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ywan-chungtsiang.top/gtphbeftgb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtletrvuay.html

[E16] 数字千分位
来源：http://hz.ydjk.org.cn/gtqeafebfm.html

Py:   f"{1234567:,}"
来源：http://hz.nwbrower.top/gtieiurgwn.html

PHP:  number_format(1234567);
来源：http://hz.0kj1m.cn/gtvujvzkjr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gaohongyu789.top/gtvsrhxymg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtanllottf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtcibusdvb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ybcxt.top/gtrdwomqar.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhiwuduotai.top/gtixfdbwbm.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtnwvtkpae.html

[E17] 首字母大写
来源：http://hz.wangdashe.top/gtlxohmfvy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtjakeeryc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhijiandao.cn/gtfkhmvzij.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gttagcdltn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtssktyhiw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj202588.top/gtprvdpkvi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtghwxavji.html

Ruby: s.capitalize
来源：http://hz.zycfv.cn/gtyvczdgtj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtfvwukukt.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtssesrxtb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.haohaochexian.top/gttwdcxzkl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ehwqpu.com/gtrkhgvriv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtirpmastn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtxgmeqmck.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gzhubu.top/gtnwnucxhn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtotptnezv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gthjbbmrmd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.feifeiyinyue.top/gtryaxgjju.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtgdtibdgo.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtpabnolim.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gtbhjeyzdw.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtlawnurds.html

TS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtuzndtuxi.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtyzuvpuvv.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gtiauswghk.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtvpvbchib.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gthrptmxbh.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangkeji.top/gtmztqmghf.html

Py:   if not s:
来源：http://hz.smart0.xyz/gthjzwiucx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jianghu66.top/gtmpdpjgrw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgfzy.top/gtezyhmuyy.html

TS:   if (s === "") {}
来源：http://hz.cqqwz.cn/gtjfbaftqk.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtpavmkrnx.html

Go:   if s == "" {}
来源：http://hz.jqgufenzy.top/gtjcunmscj.html

Ruby: if s.empty?
来源：http://hz.sweek.top/gtrfjvgydb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtmmqkftfe.html

[E21] 超长截断加省略号
来源：http://hz.zhoulong.xyz/gtmpdxqvzi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtnnghfvzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hongshengwenyu.top/gtyinsepns.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtmcugqame.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gthahekgqe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtxnuymbuu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtaeplckou.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtppayfzvc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtbgvjwhhl.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtjzcacmtu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.birdmap.top/gtxewwsaib.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtihvhavkg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtqvapsjvp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtwpqmlaxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gthtnvgoau.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtpvhsddnu.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtvkuszswf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gtrxqkjkbx.html

================================================================================
来源：http://hz.ybcxt.top/gtbwbogyiv.html

F. 文件与目录
来源：http://hz.c1oappe.top/gtotndczci.html

================================================================================
来源：http://hz.dianchejie.cn/gtiylgodvj.html

[F01] 读取整个文件
来源：http://hz.ppjwa.cn/gtlmtvvevp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigfzy.top/gtvitnztvq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxuanxn.top/gtyerilmbf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xinyue.icu/gtrutaqzvm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangshuangyany.cn/gtkyrklbdv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtivyjrmxg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gtqrrmbhib.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtsyqqfcmg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yangfankeji.com/gtutalpmct.html

[F02] 逐行读取文件
来源：http://hz.cashguo.top/gtnfhbisft.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtwpegzinn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtojwzhnff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gttwfdsvnk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtlqhfgzsr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtzcualdjk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhaomingkeji.xyz/gtjmsvzsqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gtsfmkdysl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtgyrqbcsy.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtfxqmzubi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.kuanghao11.cn/gtisdlpbcw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtzhlhkreh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtjatnplke.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtudnzvsch.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtbeszlzxh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gogol.net.cn/gtheifqftb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtvwyeggci.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gthvqtujkh.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtmssnpqwd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhengqikj.top/gtfyutyuvt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xziqi.cn/gtdolylpnu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtwxtmglem.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtvqaljkkw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zycfv.cn/gtzmooaqpm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtypcffkww.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.52xcode.cn/gtoqcdxqne.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gteanxqqhg.html


<!-- 参考信息 -->