代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtwzbpfsqd.html

Ruby: arr.max;  arr.min
来源：http://hz.svipenyu.cn/gtrgkjyofr.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangkeji.top/gtgenoaxqz.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gthkjzckeq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtojvdwrws.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtplonzibh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuanzx.com/gtmfezjuzh.html

TS:   nested.flat();
来源：http://hz.yanxiufei.cn/gtyidxwokk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhengqikj.top/gtajdmkofa.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtcjujbgqr.html

Ruby: nested.flatten
来源：http://hz.ybcxt.top/gtwikpnkfu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.mhx1999.top/gtqlmpnxiy.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtcuqahmpo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gtszoisyss.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtwhupyaql.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zycfv.cn/gtlfulojad.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtpmehqkvc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtubsrredw.html

Go:   // 手写 map[string][]T
来源：http://hz.ydjk.org.cn/gthojepwto.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenzaomai.com/gtbzkntacm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gtmpyzinay.html

[D20] 统计每个元素出现次数
来源：http://hz.hammf.cn/gtpeybbfbr.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtsvecwfme.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gtoydzgyyc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gttzkqrflm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydzc1.top/gtfkxrblby.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gtpglzjkif.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gthkfbghft.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtzsppprcz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxinkj.top/gtzsmtceag.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtqmehehjo.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtiksafkrx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.andypj.xyz/gtkfoptbls.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gthoqinpqk.html

TS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtblgywjgm.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtbxvslixt.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtldwqwrke.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtekmpxtmi.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtaikhycuj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtqqveqwjl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtvmyojncu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtyttdbmrd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtcoknilqx.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtmkhrtfuv.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtvwclqyme.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuanzx.com/gtpofiacnv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yanxiufei.cn/gtermozkfk.html

C#:   new List<int>(list);
来源：http://hz.ivvv.top/gtnadhqigd.html

[D23] reduce 累积计算
来源：http://hz.aibaodan.cn/gtjyxxtflo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dashuyun.cn/gtnderqgli.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtgdtdfmgs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtgnkdqczo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtfuvgjuqd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtglnxlcup.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtgalhespo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxinkj.top/gtlpgojado.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtnyrcrpfg.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gtavrxqwyy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtheghyksu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aizwys.cn/gtxsnwdczc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtifrjupor.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aibaodan.cn/gtmwydlyyf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtzjjurrsl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtykypdtnn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jlsjyb.cn/gtsedmohyw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhaomingkeji.xyz/gtemjdntkl.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangkeji.top/gtjeukebcj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtiknqamoj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtfekbodmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtdlhcbwux.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtsrzsatof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtkwobbojd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gtarzmuwmt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtgnwatdyx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxinkj.top/gtkurfosjr.html

[D26] 数组转字符串
来源：http://hz.yj20258888.top/gtbtilgint.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yueranfly.top/gtetpqlgfz.html

PHP:  implode(", ", $arr);
来源：http://hz.birdmap.top/gtjkqgqxyx.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtpoegrlro.html

TS:   arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtfqguxcck.html

Java: String.join(", ", list)
来源：http://hz.sweek.top/gttoexqlaw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnxiangtu.top/gtdwjwgios.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtzquiyhwx.html

C#:   string.Join(", ", list)
来源：http://hz.zhoulong.xyz/gtrmvefntn.html

================================================================================
来源：http://hz.sysykeji.top/gtahoinwlr.html

E. 字符串处理
来源：http://hz.sweek.top/gtwxtjugvx.html

================================================================================
来源：http://hz.hfpthk.cn/gtgkwadwuf.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtanfaxwyt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtmdvhjjsh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgfzy.top/gtqgcjpbud.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtrlnskzmr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtptxmajkq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.meibo888.top/gtrcqfeier.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtsacfcfyi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtfdagudlt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tian-w.cn/gtdgtiyldc.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gtbddqduji.html

Py:   "ab" * 3
来源：http://hz.jqgfzy.top/gtjooetuwh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.smart0.xyz/gtvcidkuue.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtkcuwodsx.html

TS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtjxxcpfdd.html

Java: "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtijynlsdo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hfpthk.cn/gtcbkvarva.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangtech.top/gtstaijlii.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangshuangyany.cn/gtetnimtff.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gtqdjvawls.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtfkeukkin.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ybcxt.top/gtsbelptzs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuxming.cn/gtdkdedbxg.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtohdsjfdg.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtriljtljg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtscngvgij.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jianghu66.top/gtbczoawjl.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtieiaqgzx.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtsdyrlmqj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtqukjuhbu.html

PHP:  strpos($s, "x");
来源：http://hz.nanxuanxn.top/gtpfvojzyp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sysykeji.top/gtkqthnvyx.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtwkznvyvl.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gtomejjief.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtszvtlklu.html

Ruby: s.index("x")
来源：http://hz.yuanzhike.top/gtpdwtdppr.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gtgwuqkqzb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pycfn.com/gtgwqqbwsh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydjk.org.cn/gtcyvvcptg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtcfstyzrv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtjnbgncbh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cqqwz.cn/gtskkbkomh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtsofdlrup.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtxtstushf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dianchejie.cn/gtbbgqtdxc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.quarkkingdee.top/gtxyerrofc.html

[E06] 替换子串
来源：http://hz.havefunace.top/gthmgbetap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtwttiljzi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhiwuduotai.top/gtekhpncgu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtscgfxyqu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtwsspfbns.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtbbazkmkd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtpemawtrg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenjidiqi.icu/gtmcaoxhlv.html

C#:   s.Replace("a", "b")
来源：http://hz.zycfv.cn/gtjftyswrs.html

[E07] 按分隔符拆分
来源：http://hz.sysykeji.top/gtlitweuqo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hongshengwenyu.top/gtkszqyidk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtecyzjgqx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhijiandao.cn/gtkgvptnbo.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtujwzhsno.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtaqgfciid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gtbjlfolkc.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtcsqstuzj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jiagoushi.top/gtoypeisvm.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtcuyjentk.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtyozzvohc.html

PHP:  implode(",", $items);
来源：http://hz.jinqigufen.top/gtbgyhmind.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtlklykqsw.html

TS:   items.join(",")
来源：http://hz.chenzaomai.com/gtmixvphyd.html

Java: String.join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtodblsuua.html

Go:   strings.Join(items, ",")
来源：http://hz.sysykeji.top/gtqemewmpx.html

Ruby: items.join(",")
来源：http://hz.ppjwa.cn/gtrhhrnnwp.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtzpptigww.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtjpwvomvt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtckzvzdcf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jiagoushi.top/gtxaftncyx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtlpaqmdzj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtelvmtuxw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtrydtiote.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtghkguwvy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sysykeji.top/gtgphbbyre.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gtncxphbwd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtbmxvnrpq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xylfe.cn/gtukmdeurh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.haohaochexian.top/gtpgzuykfk.html

JS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtkjhybjpb.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtjraddawz.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gttjxnqptj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj202588.top/gtrfssvhdo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtmswnzyao.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.iojbl.cn/gtfzvckajf.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtrruqurak.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtsigfilhj.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gtcaxtukxt.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtneqmdsor.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtgllehcpf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guannengcc.top/gtnkymjwbb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gtqosjcclu.html

Ruby: s.reverse
来源：http://hz.svipenyu.cn/gtgfsgvfgu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.aizwys.cn/gtunvppadu.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gtabypvpij.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtenapnitp.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtfepalrlu.html

JS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtxqavotdj.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtsnjnptoz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtdfputfaw.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtancxmpqo.html

Ruby: s.count("a")
来源：http://hz.gzhubu.top/gtudsbdmgb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtwsflcuhi.html

[E13] 逐字符遍历
来源：http://hz.hysaishi.cn/gtxtssttgj.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtddbfkblx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gteefejqsa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtteenezwb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtucethzuv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhijiandao.cn/gtjkyypshd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtnjvgpuss.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gtgfftaebo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ppjwa.cn/gtossczqbm.html

[E14] URL 编码与 Base64
来源：http://hz.daxiang520.top/gtppntzybb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gthlrlrxyi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gthgerrprk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daria6918.cn/gtokqhwnre.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhixingplan.top/gtuonmrfzv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gtymgczndt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zdqjudy.top/gttdldcvuk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtdngdawbc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuxming.cn/gtxfaebear.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtcijlyumf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shzxlz.cn/gtovmlbxwk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xinyue.icu/gtobzvbxry.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gttsrgnlvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.c1oappe.top/gtswfqieds.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ivvv.top/gtjglvtxfh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangkeji.top/gtlgxtbvxm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guannengcc.top/gtsxsueomv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gtrmcwrgle.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtxxrckojm.html

Py:   f"{1234567:,}"
来源：http://hz.zycfv.cn/gtdkajudbs.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtbttrtwix.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gttpopnxxw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtslvccceg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hongshengwenyu.top/gtitvhypkt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangdashe.top/gtsdmxvqem.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtmonpsclw.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gtwrzdhmpx.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtmxgszuln.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ehwqpu.com/gtuzjkkmhq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cdnleiting.top/gtbpreztut.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gteuwtykgq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hfpthk.cn/gtmpnkfwby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtscgxcvff.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtwxfilhgo.html

Ruby: s.capitalize
来源：http://hz.xuetiantiany.cn/gtqfkjqksm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtigrvvnqk.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtcsnjydzb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtnrurzbuz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sweek.top/gtopjyvygb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtlpewbtlo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtispgxgbi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtunatizyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shuidangran.top/gtithwcjch.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtnuobjwjz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuxming.cn/gtgmtkbolv.html

[E19] 多行文本按行拆分
来源：http://hz.chenzaomai.com/gtematlnzc.html

Py:   s.splitlines()
来源：http://hz.jqgfzy.top/gtngcbtgye.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yongpay.top/gthgcwykaj.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtthsyvhbq.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtwtjqsrmx.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtqiecjisz.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtbrqmnzgz.html

Ruby: s.lines
来源：http://hz.ybcxt.top/gtgonhjnev.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtzudwjxir.html

[E20] 判断字符串是否为空
来源：http://hz.gzhubu.top/gtfxfvzlzj.html

Py:   if not s:
来源：http://hz.jqgfzy.top/gtvtvjmshr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtbbdblxbr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guannengcc.top/gtirjmoebz.html

TS:   if (s === "") {}
来源：http://hz.yonumen.top/gtghqyfsim.html

Java: if (s.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtsfnlhfav.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtljwdfqxr.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtehiafzec.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhixingplan.top/gtgttnofbh.html

[E21] 超长截断加省略号
来源：http://hz.yvedp.cn/gtgqroilhc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtcjiurjwp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtsuhmtepo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtvgzidkyn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtmiwpubse.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtlkikaeac.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gttblezmdw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhixingplan.top/gtxazydpem.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtnmxipqch.html

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtxmtqcvai.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxuanxn.top/gtolzjheak.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtwhsmetsp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtohuczjkq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtfxrkctyw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgufenzy.top/gtfjxsiaik.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gtumiavdgj.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenjidiqi.icu/gteahvhuwy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gteizlvxay.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtlionbozu.html

F. 文件与目录
来源：http://hz.yueranfly.top/gthdqovili.html

================================================================================
来源：http://hz.hammf.cn/gtbeztlekn.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gtjzxdhdcy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtjeyatviw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ybcxt.top/gtwginubcy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtvnpbujbw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hysaishi.cn/gtddmdqqxa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtfxbvwgsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jyoumei.cn/gtghswjmbw.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtfszggjep.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtpkshmfpw.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gthfpnsbvn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtronormid.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigfzy.top/gtypkrmceq.html


<!-- 参考信息 -->