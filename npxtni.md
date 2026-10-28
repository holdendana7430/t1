代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gttsphlxlc.html

[D20] 统计每个元素出现次数
来源：http://hz.shangyingyoupin.top/gtsfdbblmq.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtrvhgsyrk.html

PHP:  array_count_values($arr);
来源：http://hz.jqgfzy.top/gtehdeeqdp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gttoiavpkq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtebqipgmu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtofyfydxb.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtnkwynode.html

Ruby: arr.tally
来源：http://hz.hnxiangtu.top/gtoioizfbi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daria6918.cn/gtmzmtqijc.html

[D21] 判断是否包含某元素
来源：http://hz.xinyue.icu/gtztvjzvyh.html

Py:   x in arr
来源：http://hz.wangdashe.top/gtdwcmaqpb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtkllonapl.html

JS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtumlspojt.html

TS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtmhlnphva.html

Java: list.contains(x)
来源：http://hz.xuanzx.com/gtmosrggak.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtampgbzle.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtofytkrcv.html

C#:   list.Contains(x)
来源：http://hz.dianchejie.cn/gtrtvogpgg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hammf.cn/gtvfuwfppf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangshuangyany.cn/gtimvkxzvy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jyoumei.cn/gthrgzwgay.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenjidiqi.icu/gtzgudxxnq.html

TS:   [...arr];
来源：http://hz.sufxvd.cn/gthwrkahbo.html

Java: new ArrayList<>(list);
来源：http://hz.gzhubu.top/gtviymxmqu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.vqdsnc.cn/gtvtxjdkpg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gzhubu.top/gtddttsbea.html

C#:   new List<int>(list);
来源：http://hz.iojbl.cn/gtfyreegij.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangtech.top/gtrcebpecm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtsjmhdhtl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.haohaochexian.top/gtekedpqvq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gthxpdgslc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtmjicsxal.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ywan-chungtsiang.top/gtlatdlgvi.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtncmggkjv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtewmwsxow.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gteyjtosni.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtegtqhdwp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtepuwfbxb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtxrpyulvt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangshuangyany.cn/gtygardxiz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenjidiqi.icu/gtrarvvvzl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yueranfly.top/gtagdqgpfo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tanke756.top/gtfuujkfkh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xziqi.cn/gthibyqcyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtwfquqefb.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtxhmbkhwb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.haohaochexian.top/gtjdrhdfnd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.andypj.xyz/gtvjlrabgs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gaohongyu789.top/gtvcuqjqzr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gtyyolcpod.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtgoysjqtn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtmduxwlcz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtmddgkdhj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ywan-chungtsiang.top/gtgwwwvsdz.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtiwoxrwem.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gtqrqdipvo.html

PHP:  implode(", ", $arr);
来源：http://hz.andypj.xyz/gtecdwrnla.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtcdbecbrs.html

TS:   arr.join(", ")
来源：http://hz.xylfe.cn/gtogxxdirx.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtpjmilmii.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zycfv.cn/gtpyaiaiqv.html

Ruby: arr.join(", ")
来源：http://hz.andypj.xyz/gtqghvwmir.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtltknxsqc.html

================================================================================
来源：http://hz.sysykeji.top/gtovzohfta.html

E. 字符串处理
来源：http://hz.shanyushiyangtech.top/gtbrjddgyx.html

================================================================================
来源：http://hz.sxryk.cn/gtmfrbaarz.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gtbabdthht.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtjsrdsjew.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinghuilouyu.cn/gtffdrjhzw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtwcnftvnt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtpexmjwyu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gotoacloud.top/gteqxbhkgl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pycfn.com/gtudtlefkb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yueranfly.top/gtnpsktxqs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtdmzzopoe.html

[E02] 重复字符串
来源：http://hz.c1oappe.top/gtpiglkkmr.html

Py:   "ab" * 3
来源：http://hz.guannengcc.top/gtixigsdpc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jianghu66.top/gtpuidwptc.html

JS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtrpwwevut.html

TS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtfidsqcvr.html

Java: "ab".repeat(3)
来源：http://hz.yuxming.cn/gtbyxqlvmy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhoulong.xyz/gtoppibxpd.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gtxtchimun.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtqnyrwoep.html

[E03] 截取子串
来源：http://hz.jqgufenzy.top/gtbdadwhll.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jlsjyb.cn/gtdifwzuvv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gtyntnzxny.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jianghu66.top/gtcrafblgk.html

TS:   s.slice(1, 4)
来源：http://hz.yangfankeji.com/gtzmhvldqo.html

Java: s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtbrjcpzpa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtaigymwcp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gtvfcnxudw.html

C#:   s.Substring(1, 3)
来源：http://hz.tianlin.xyz/gtvzdbskjs.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtlkbfojxj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shzxlz.cn/gtxrpwnglh.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtibxrbdrn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinqigufen.top/gtvgldqynz.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtunmptnuo.html

Java: s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtfbjdkchd.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgfzy.top/gtanduklto.html

Ruby: s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtzwwblotv.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtpkxobxoy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dianchejie.cn/gtatvhfsex.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yanxiufei.cn/gtzldizycb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hywenlv.cn/gtiittkhql.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtqqwhqolu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xuetiantiany.cn/gtdscocajp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yongpay.top/gtbjyjyhia.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj202588.top/gtzwucglae.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pengpengdd.cyou/gtgpiqvcax.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtetxwxvfp.html

[E06] 替换子串
来源：http://hz.ppjwa.cn/gttldofabb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxinkj.top/gtrnnznyqa.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.daxiang520.top/gtnfqpkvnc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtbngjblsm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtxtlmatuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtzsldmjlb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guowangkeji.top/gtxnsvvekp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.mhx1999.top/gtylmfikmj.html

C#:   s.Replace("a", "b")
来源：http://hz.zhongyouzk.top/gtbuvaszlg.html

[E07] 按分隔符拆分
来源：http://hz.havefunace.top/gtlakmksul.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhiwuduotai.top/gtokwqungd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtvjxkzuyf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuetiantiany.cn/gtrbeiviqv.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtsgjccqcy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnqzz.top/gtfvascncb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xylfe.cn/gtzsmxmakp.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gttjpmxuiy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sweek.top/gtaupkjifi.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtpjlnhgtt.html

Py:   ",".join(items)
来源：http://hz.hnqzz.top/gtaldmkqud.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gttqlyrrxh.html

JS:   items.join(",")
来源：http://hz.cucudq.cn/gtxyibfqoz.html

TS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtvkjzgefx.html

Java: String.join(",", items)
来源：http://hz.zhengqikj.top/gtildwqrim.html

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gtjowkuxzi.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtbbqhqyoo.html

C#:   string.Join(",", items)
来源：http://hz.daxiang520.top/gthzqcnaqz.html

[E09] 去除所有空白字符
来源：http://hz.smart0.xyz/gtqwsvugmd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cqqwz.cn/gthcufyyah.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtvinrbhbf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtivjkjiaa.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sweek.top/gthqgkwcjp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gttcrhlseg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtzledsfzh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gtbohjdjbd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.quarkkingdee.top/gtxpxzkrei.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtrnmhlqau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hysaishi.cn/gthbihusry.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jiagoushi.top/gtgxghbuuo.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtfisaiovt.html

TS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtelqowpby.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtnlmjrvbu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gthueiseqi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtxfugyngr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtbvuxlgwh.html

[E11] 反转字符串
来源：http://hz.yanxiufei.cn/gthtlufqti.html

Py:   s[::-1]
来源：http://hz.pycfn.com/gtdncyrgba.html

PHP:  strrev($s);
来源：http://hz.zdqjudy.top/gtvkxyzdwd.html

JS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtxksdaufs.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtasfjgldg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yonumen.top/gtysmmxazw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gtawknhtgg.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtujcyyokk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtgazgehrs.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtpdlicagi.html

Py:   s.count("a")
来源：http://hz.andypj.xyz/gtpqpeycfo.html

PHP:  substr_count($s, "a");
来源：http://hz.vqdsnc.cn/gtmxbhivxx.html

JS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtsmnajavb.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtmevzmblc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shangyingyoupin.top/gtepnzfmgz.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gtktlijpcd.html

Ruby: s.count("a")
来源：http://hz.316326.xyz/gtpfeszcby.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shangyingyoupin.top/gtnndspaxg.html

[E13] 逐字符遍历
来源：http://hz.yj20258.top/gtqqhkkxit.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtqlompesr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtfqaaecgt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtbjsmnjjx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gaohongyu789.top/gtpuqgeosw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtdjwwunua.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtwykweybz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtkeolxdrl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ppjwa.cn/gtokgoeahn.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtklmyjqmd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtpyhsjjdv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtwwsznbbj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnqzz.top/gtefhhvnfe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtdhrzylrm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jlsjyb.cn/gtikdfnbcv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daria6918.cn/gtxpwkzchx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sufxvd.cn/gtajhbddnn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtouiipxuj.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtarjgkbjm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pengpengdd.cyou/gtgdlwtnfq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jiagoushi.top/gtyfiktpqq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtyycoivcx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jianghu66.top/gtztwpojay.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gtyhfhwklh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daria6918.cn/gtpswyfgvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtaoaomqln.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtyulryrzw.html

[E16] 数字千分位
来源：http://hz.pengpengdd.cyou/gtvdtorrwm.html

Py:   f"{1234567:,}"
来源：http://hz.hywenlv.cn/gtufqdhlfy.html

PHP:  number_format(1234567);
来源：http://hz.0kj1m.cn/gtlsonpvgc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gteejdhtow.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtayvgrnwb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guannengcc.top/gtieisxvje.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhengqikj.top/gtgjkjweun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.meibo888.top/gtiiufkkpo.html

C#:   1234567.ToString("N0")
来源：http://hz.yongpay.top/gtsskwttlm.html

[E17] 首字母大写
来源：http://hz.tanke756.top/gtorsfekeu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtwsbimzme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtrmabeelm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtdxjqquyn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtwlmwosau.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhixingplan.top/gtrhzrtwnf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sxryk.cn/gtxyjlnaus.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gtfgfqccur.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtambezbuz.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtkewwenwm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtafcpjmbe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shanyushiyangkeji.top/gtuvhpwoax.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtfqwwumem.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtfsdnkitn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtllqzhqra.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtmyfwgmds.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhaomingkeji.xyz/gtsujxqyvv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtejahuaga.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtqswfgsei.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtanugajlo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtjcdbhafj.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtilljqidk.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtnebmtzii.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtpjrnvjgt.html

Go:   strings.Split(s, "\n")
来源：http://hz.ybcxt.top/gtkhxihaaf.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtcknkkfzo.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gtczgexyzo.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtdgjexqdr.html

Py:   if not s:
来源：http://hz.xuetiantiany.cn/gtghsuoihu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtnmlyvclc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hywenlv.cn/gtcvfnjfcs.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtjyscgzgp.html

Java: if (s.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtxywyislb.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtegkpuoaj.html

Ruby: if s.empty?
来源：http://hz.zycfv.cn/gtpjcydbzd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.iojbl.cn/gtxbaxvrzw.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gttcojcmel.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yangfankeji.com/gtjgtblxga.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cdnleiting.top/gtcuovovfx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtyxvsuenh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gthszwpqcr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtworepkwl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtzfmwpouv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shuidangran.top/gtkwgrquns.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtjxpowtgj.html

[E22] 字节长度与字符长度
来源：http://hz.xinyue.icu/gtrzvylike.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aizwys.cn/gtcntegtcj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtxdeaurjr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtpvobweeu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtybtrnqvx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtjbmqtnku.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gtnyjtbnyy.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtxoxthawb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gtrqpekmqj.html

================================================================================
来源：http://hz.zhixingplan.top/gtydqqcwxb.html

F. 文件与目录
来源：http://hz.hysaishi.cn/gtewflithm.html

================================================================================
来源：http://hz.nanxinkj.top/gtncgfdlip.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtojcvfpbd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtsxguedso.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtorufwedj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gtgkhwryuc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.meibo888.top/gtpjhiprih.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtaywmxojv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dianchejie.cn/gtajbbnaij.html

Ruby: File.read("a.txt")
来源：http://hz.xinyue.icu/gtholyfsnq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinghuilouyu.cn/gthclsrpme.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gthlharzlo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtvepvqohv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtmwdhkcre.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtizrybnxa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtarzkrjow.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtujmjvqbv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtlolnkygh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gteyuquqjq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtuqostoih.html

[F03] 写入文件（覆盖）
来源：http://hz.guowangkeji.top/gtmbdoolli.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cashguo.top/gtndipjyep.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj202588.top/gtqawcbnkt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtkaooqgjx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtkihhoymk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtsdqlhrsf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jianghu66.top/gtrsjxjxhm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.redwolf501.top/gtxawqosov.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tian-w.cn/gtnwvnbveu.html

[F04] 追加写入文件
来源：http://hz.9152youxi.cn/gtazffhphv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtiqibllgq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtsmhvsjmj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtwwslgllm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtfpbgyxuf.html


<!-- 参考信息 -->