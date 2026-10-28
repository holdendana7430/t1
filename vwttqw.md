代发 wailian999

[D19] 按字段分组
来源：http://hz.zycfv.cn/gtimrekyyz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.kuanghao11.cn/gtqxstqmjg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gtjcjpuocb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gttgyuiiyt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gtaslawbbm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtjqoawyvj.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtkevslvrv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jianghu66.top/gttqceyqou.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtobzwlfwv.html

[D20] 统计每个元素出现次数
来源：http://hz.yongpay.top/gtujkqnund.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtgsmixqxj.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtaaefssqv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtcdwlqrdl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtbkduorye.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tian-w.cn/gtmgwokzwb.html

Go:   // 手写 map[T]int
来源：http://hz.nanxinkj.top/gtutnqqykn.html

Ruby: arr.tally
来源：http://hz.xingfuxueyuan.xyz/gtyspxmkmw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtijngmzch.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtohulqldd.html

Py:   x in arr
来源：http://hz.0kj1m.cn/gtlmhiyfga.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gtqvoivkbx.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gttrjjhdak.html

TS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtiesxoogw.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gtcpkcdqwu.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtlwiudfei.html

Ruby: arr.include?(x)
来源：http://hz.cdnleiting.top/gtoflvvkic.html

C#:   list.Contains(x)
来源：http://hz.jlsjyb.cn/gthuxfjrzt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gttiodigsi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtcqyoutqw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.dashuyun.cn/gtrbftmbhg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daxiang520.top/gtqnzbryyn.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtlwyywngd.html

Java: new ArrayList<>(list);
来源：http://hz.meibo888.top/gtouqzhdmc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xziqi.cn/gtxcsmghts.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtobbgdvdf.html

C#:   new List<int>(list);
来源：http://hz.tanke756.top/gtmwyrurov.html

[D23] reduce 累积计算
来源：http://hz.hnqzz.top/gtcjioxetg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtfxirvelo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtgigqxqds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtkbwnexxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtspdjuijo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yanxiufei.cn/gtyodjlgyj.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtvhhenyhc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtqrpmaegd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jiagoushi.top/gtvxzuvdvx.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgufenzy.top/gtkzhwrjfb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgfzy.top/gthsqihpep.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hywenlv.cn/gtxteaarbg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtjubvduqd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxinkj.top/gtvlbldmqg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gtcklqdkpb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tian-w.cn/gtfaqghter.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yueranfly.top/gtgrxurwew.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daria6918.cn/gtvxuickzp.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtrgvvgopc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtzeudfipk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtmppersve.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.kuanghao11.cn/gtxidvfdio.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sufxvd.cn/gtmaenptit.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxinkj.top/gtrtktrzno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gttqakpimg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtgiulzujp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtyfqaxnog.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtrfbacdhu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtyandnxmj.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gteucjfhzk.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtbczphggk.html

TS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtldceecua.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtrknepfff.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtrgksucps.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtuylxjyhg.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtilubzkok.html

================================================================================
来源：http://hz.yuanzhike.top/gtfgkcmaov.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gthureawsf.html

================================================================================
来源：http://hz.aizwys.cn/gtrzjmmffy.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gthsbwsrbo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.snrcjt.cn/gtqaxzmrvd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtsobcjcxe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtnryotbxz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtjyapprih.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hongshengwenyu.top/gttzvohahs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtjlauecop.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhijiandao.cn/gtsjsxzfve.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.quarkkingdee.top/gtacmwxmwh.html

[E02] 重复字符串
来源：http://hz.hongshengwenyu.top/gtqshpszmj.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gtjoavcmlu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtnaawzctb.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtahjcrvoa.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtfxdchalc.html

Java: "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtxdzuefyw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gtqlsfxtul.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtkgoatgnl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtxdnrbsat.html

[E03] 截取子串
来源：http://hz.gotoacloud.top/gtbveyrrzf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtpqtypqcd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gturlxmgud.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zycfv.cn/gtxngzmfdd.html

TS:   s.slice(1, 4)
来源：http://hz.sufxvd.cn/gtlqeazjmr.html

Java: s.substring(1, 4)
来源：http://hz.iojbl.cn/gtadfriydf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj202588.top/gtbtqxdjug.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gtndkuxuxs.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtjypttcox.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtsnvkuquu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj202588.top/gtzreoqnpt.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gtfblestll.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.iojbl.cn/gtfeedsknw.html

TS:   s.indexOf("x")
来源：http://hz.mhx1999.top/gtxzvkyagc.html

Java: s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtyxzncwcm.html

Go:   strings.Index(s, "x")
来源：http://hz.redwolf501.top/gtjfztaqsf.html

Ruby: s.index("x")
来源：http://hz.zhoulong.xyz/gtdwujtzjv.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtcmujxntc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tanke756.top/gthabvwmce.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ehwqpu.com/gtanibhrjy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shuidangran.top/gtsxxbmcxh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtlpxbhxhc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtrevegoyv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtsrzkgfxp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtyvkoyzeo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jiagoushi.top/gthmnwskot.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.iojbl.cn/gtfcblxoqe.html

[E06] 替换子串
来源：http://hz.iojbl.cn/gtkefzbsfj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgfzy.top/gtjgclbnwe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangtech.top/gtanzttlex.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtxgimrnpn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtbajysxnl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gthlvuxcmb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daxiang520.top/gtrgwogmtg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.feifeiyinyue.top/gtbctfwtcm.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtrimfsfbi.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gtbwlrotqb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtklquftvi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtugoikzrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhongyouzk.top/gtsxzwdrqn.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gtupnmoykm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtlsxkmlux.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yonumen.top/gtzcdzmxia.html

Ruby: s.split(",");  s.split
来源：http://hz.quarkkingdee.top/gtefltxfze.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.havefunace.top/gtfstsqtbk.html

[E08] 数组按分隔符合并
来源：http://hz.shzxlz.cn/gteznrlqyt.html

Py:   ",".join(items)
来源：http://hz.birdmap.top/gtgxufgshn.html

PHP:  implode(",", $items);
来源：http://hz.hfpthk.cn/gtsiukemqy.html

JS:   items.join(",")
来源：http://hz.aibaodan.cn/gtjmvfswct.html

TS:   items.join(",")
来源：http://hz.jinqigufen.top/gttofllvrt.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gttkkvhdtg.html

Go:   strings.Join(items, ",")
来源：http://hz.yuanzhike.top/gtikacjbcc.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtyftrysfj.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtsohsmudw.html

[E09] 去除所有空白字符
来源：http://hz.xziqi.cn/gtyiflvqev.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhoulong.xyz/gtinacozml.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hammf.cn/gtkpoptywh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtvbgvbzxo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtzaluavfw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shuidangran.top/gtsbvslush.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtfedqaeny.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xingfuxueyuan.xyz/gtgdfhrqad.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtqsbabpzm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yangfankeji.com/gtblalndbl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ehwqpu.com/gttqmotalr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gtmrjbcqrm.html

JS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtugjgwjnh.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtoaufsqzn.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtjtgjvbua.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nwbrower.top/gtnuijtlyu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtdvzjouga.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtavejxdrv.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtvnswrlwr.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtbdttmmtr.html

PHP:  strrev($s);
来源：http://hz.hfpthk.cn/gtplmknjjs.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtuuhlrvaj.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtzrhqvpqo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtcjwpojce.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gtbvsqcvtu.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtbvbzvwot.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtpvcsyjkh.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtphzqbgco.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtkfppfqgn.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtmrzzaavl.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtphyqezkm.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtisquwlvr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtaeadnqkp.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtypgdybww.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtgcrbhhsh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtyyinrjhl.html

[E13] 逐字符遍历
来源：http://hz.tian-w.cn/gtwmlxptxl.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gtsnsvdnfb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtumgxrvsz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtbskiaezk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtgvugxzbb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtoaipybfq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gtoowmnvbq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtsfootvmn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtqakzlyjw.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gtcukxofkl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtmlbjkilw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtpukmocti.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtuasdoaim.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtakutzdvm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuxming.cn/gtwemfuhuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgufenzy.top/gtzznlywxh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yueranfly.top/gtelfpdbfj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hfpthk.cn/gtvqwfohgh.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtormbtoit.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtgjqdiysu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtfolsiyzg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258888.top/gtgzzrjgzh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgfzy.top/gtkarsildz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtgcojvxkn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtvvlxxqqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhaomingkeji.xyz/gtmjirwlrf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtnaxydsej.html

[E16] 数字千分位
来源：http://hz.wangshuangyany.cn/gtmtxataio.html

Py:   f"{1234567:,}"
来源：http://hz.mhx1999.top/gtbevkclgk.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtlltjmqsl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtrjrowhgz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtexvuwhto.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zdqjudy.top/gtrovznchf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gteblqmsml.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuanzhike.top/gtkdhynrra.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtwrbnnzyd.html

[E17] 首字母大写
来源：http://hz.nwbrower.top/gtgxaiafdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hfpthk.cn/gtnoduridh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigfzy.top/gtzerpngrd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtdhlfpizo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtqvjsrvkz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dashuyun.cn/gteywgbbet.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gtowwifziu.html

Ruby: s.capitalize
来源：http://hz.316326.xyz/gtkdyvejwz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtvmsjgivy.html

[E18] 模板占位符替换
来源：http://hz.iojbl.cn/gtcvdqidaj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhengqikj.top/gtdcivsvpu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtukdusbjl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtqezoosuc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtodecjpzk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gtklammkkm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtydpnmgcx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtfgcvekfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yongpay.top/gtgixjqfav.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtnbbdekei.html

Py:   s.splitlines()
来源：http://hz.guannengcc.top/gtagxcghlj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yongpay.top/gtstxpiiwa.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtezstbzrn.html

TS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtqqcuikkd.html

Java: s.lines().toList()
来源：http://hz.nanxinkj.top/gtndxgrctk.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gteifpiquj.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtevgczsfk.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtmjkrekbh.html

[E20] 判断字符串是否为空
来源：http://hz.sxryk.cn/gtpcvpnzgz.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtbnnudzuz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gtcrjizjwv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtltjgovid.html

TS:   if (s === "") {}
来源：http://hz.nwbrower.top/gtbcryceup.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtscuegjlh.html

Go:   if s == "" {}
来源：http://hz.9152youxi.cn/gtyrakvyva.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtagdyjgsg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtkbnwufqh.html

[E21] 超长截断加省略号
来源：http://hz.meibo888.top/gtwvsgptwm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj202588.top/gtslmcwjgk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pengpengdd.cyou/gtuoqqfljt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtwulovkuo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtkfynhrmu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtqyxlwbvk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtweqrzwmy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cucudq.cn/gtqltdjgwp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtcwnacsgi.html

[E22] 字节长度与字符长度
来源：http://hz.yonumen.top/gtpwkrhlxe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.bjfxy.top/gtpchyvdpj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtszoolfsg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtjpjwbahs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtmnihozgd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gotoacloud.top/gtqsrrocok.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtuwmonmtc.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtvajszkry.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xinyue.icu/gttdbbasbe.html

================================================================================
来源：http://hz.zhengqikj.top/gtigvlwgok.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtsobneqoe.html

================================================================================
来源：http://hz.tian-w.cn/gtuoruntsm.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtwojfyixw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgufenzy.top/gttwzmnoul.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtjtndqmyk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gttmecmpii.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.havefunace.top/gtvenfqeuv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtosgjlszi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtziqzrwep.html

Ruby: File.read("a.txt")
来源：http://hz.ppjwa.cn/gtiagvinbl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gticijarky.html

[F02] 逐行读取文件
来源：http://hz.tianlin.xyz/gthcbupezg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtjpndotxk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtmhdterxv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtijdfvgcq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtlrdxypfm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtippklguy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sysykeji.top/gtjdzoczad.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtuxijqkub.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zdqjudy.top/gtnpcjywqb.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtdcqobsvx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtslsiebrx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ybcxt.top/gtrbmftdln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtyutiacuc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtblbvydqv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ivvv.top/gtjevuhlao.html


<!-- 参考信息 -->