代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gthogopnir.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yueranfly.top/gtdspycomu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenlongwang.top/gtzswbqlws.html

Ruby: arr.uniq
来源：http://hz.redwolf501.top/gtkzpgglbq.html

C#:   list.Distinct().ToList()
来源：http://hz.svipenyu.cn/gtffetauyy.html

[D16] 求和与平均值
来源：http://hz.yanxiufei.cn/gtsontxfci.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.kuanghao11.cn/gtwanykkfa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtejbmhbwq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtjwuatuxe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtdljqqbvv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtnkagdrum.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtggexrnyo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yonumen.top/gthttwszby.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gthsnzbvsd.html

[D17] 最大值与最小值
来源：http://hz.zdqjudy.top/gtlrwgtelb.html

Py:   max(arr);  min(arr)
来源：http://hz.havefunace.top/gtzwznbfuz.html

PHP:  max($arr);  min($arr);
来源：http://hz.cheryme.top/gtlcscttqx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtqtvdgnnm.html

TS:   Math.max(...arr);
来源：http://hz.cucudq.cn/gtbjlfrgma.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtwkdahpgz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daxiang520.top/gtakrxpoxs.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtflmwhqcx.html

C#:   list.Max();  list.Min()
来源：http://hz.sufxvd.cn/gtogydpyir.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtzvxfhiun.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gtmxlqplyh.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtomlyubxd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.0kj1m.cn/gtrqimmpsa.html

TS:   nested.flat();
来源：http://hz.gaohongyu789.top/gtpjsegaoa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigufen.top/gtnxmcyyrm.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gttmsgrvoo.html

Ruby: nested.flatten
来源：http://hz.zhongyouzk.top/gtjyyyxkvg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtfsarfhbn.html

[D19] 按字段分组
来源：http://hz.cashguo.top/gtwujlhsgj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gttnbbqpdz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtgehswtqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydzc1.top/gtbkbtaqlj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtwrjgnria.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gtnhngrsdz.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtfgavwuiv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sysykeji.top/gtfwdhutgj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtllxybhso.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtbadvjcqv.html

Py:   Counter(arr)
来源：http://hz.xuanzx.com/gtzredhzff.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtrspvlmoe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtoiftobbe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gttxnnvldh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtybkuvhof.html

Go:   // 手写 map[T]int
来源：http://hz.yueranfly.top/gtlzzwkanj.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gtkovttmsr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtvarqvppa.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gtuxstrfdf.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtajejpabd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnxiangtu.top/gtzbanmvvf.html

JS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtrhpbmbyc.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtltrbsuws.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtvmbmbvfs.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtlvrtdbxo.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtidtbodif.html

C#:   list.Contains(x)
来源：http://hz.yj20258.top/gtqrtgxzvp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtewpmgopj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yonumen.top/gtapyonzla.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtzkynqqxm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuanzx.com/gtuvdpguzy.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtuwjfilmu.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gtdqpsamyt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daria6918.cn/gtqllygxww.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cashguo.top/gtjnwgyorz.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gtokmvllnh.html

[D23] reduce 累积计算
来源：http://hz.sxryk.cn/gtymvyrbcr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtehyvywcq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtuhmgspjh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtqhsxmemu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtyqdvmlld.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtaevwtmpz.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtwagkcifi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yanxiufei.cn/gtxreedllq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cheryme.top/gtrypgwqho.html

[D24] 字典 / Map 基本操作
来源：http://hz.havefunace.top/gtlazeivhg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hysaishi.cn/gtexoznabk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gtbnylxbpy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gtgwbxudmh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtcnepvicp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cqqwz.cn/gtvinfbdap.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtcghdzxjr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gtekqpyhwg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zdqjudy.top/gtupbhgrmk.html

[D25] Set 集合去重与交并差
来源：http://hz.pengpengdd.cyou/gtmciljvyp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sufxvd.cn/gtmrnbewez.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtqbptektn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sxryk.cn/gtzrinttwo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhengqikj.top/gtdytlbdwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xingfuxueyuan.xyz/gtolmncqvf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtzngzyjrp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shangyingyoupin.top/gtntdgkpww.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenlongwang.top/gtbtandlbs.html

[D26] 数组转字符串
来源：http://hz.cashguo.top/gtunrbvraj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenjidiqi.icu/gtccwjtoah.html

PHP:  implode(", ", $arr);
来源：http://hz.yuanzhike.top/gtnxkltwjx.html

JS:   arr.join(", ")
来源：http://hz.c1oappe.top/gtrmfogycd.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtpxjwwjni.html

Java: String.join(", ", list)
来源：http://hz.jinqigufen.top/gtsykkfmkq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.haohaochexian.top/gtghjvkpxv.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtudfqpafv.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangtech.top/gttzcyvjjk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtapodwakv.html

E. 字符串处理
来源：http://hz.daria6918.cn/gtpzocljdw.html

================================================================================
来源：http://hz.c1oappe.top/gtqmzkefpy.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gtcwrjrpag.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtasrkxvgs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtantgihwu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtstpqmrmz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtkzgitoin.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtotmsqhbi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258.top/gtgwtgusyn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cqqwz.cn/gthhevrmns.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.meibo888.top/gtucyzdrbw.html

[E02] 重复字符串
来源：http://hz.yj20258.top/gtzgsitonj.html

Py:   "ab" * 3
来源：http://hz.sxryk.cn/gtkikmkhfc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.svipenyu.cn/gtatwzkpcz.html

JS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtiynievkn.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtzrtasaio.html

Java: "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtdjlyyxnb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj202588.top/gtpqgtkupp.html

Ruby: "ab" * 3
来源：http://hz.nwbrower.top/gtrjzycnlg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.vqdsnc.cn/gtfcromcvh.html

[E03] 截取子串
来源：http://hz.jlsjyb.cn/gtdpphpzmu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangtech.top/gtaihzphku.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtgxftrifi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtwjquetci.html

TS:   s.slice(1, 4)
来源：http://hz.hfpthk.cn/gtusznxbwt.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtthuowtce.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuxming.cn/gtyxgszatv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gtbkzpsptp.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gtevpbqeub.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gthhsxgzwp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hysaishi.cn/gtkhcjphfe.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtmhqbynno.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.mhx1999.top/gtgbdfwexl.html

TS:   s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtmyfdamka.html

Java: s.indexOf("x")
来源：http://hz.bjfxy.top/gtzrhiqvdu.html

Go:   strings.Index(s, "x")
来源：http://hz.vqdsnc.cn/gtlszlhtuv.html

Ruby: s.index("x")
来源：http://hz.jyoumei.cn/gtrkiyrolx.html

C#:   s.IndexOf("x")
来源：http://hz.zdqjudy.top/gtjljtabdm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cashguo.top/gtlqjtywdb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yangfankeji.com/gttdubatxo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tian-w.cn/gtyjexaqzy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gttnaiwkzc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shanyushiyangkeji.top/gtytrxhruj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gtfentvatd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ybcxt.top/gtlabxrezb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtmgxfnqvm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtbpahvjdk.html

[E06] 替换子串
来源：http://hz.hysaishi.cn/gtmrpduvwc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pycfn.com/gtlhqgdwec.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ppjwa.cn/gtsmlyyyym.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtjvrrtgfu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtxhaiouft.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gttqgfnfly.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gttkqzmwgw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.meibo888.top/gtrmssxbzc.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtqwelbyaf.html

[E07] 按分隔符拆分
来源：http://hz.pengpengdd.cyou/gteaaeurys.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gotoacloud.top/gtsosoapzr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cdnleiting.top/gtujbvphec.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtaluyjsgj.html

TS:   s.split(",")
来源：http://hz.yueranfly.top/gtlpwfovmw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenlongwang.top/gtjcntzude.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hammf.cn/gtbzraxswl.html

Ruby: s.split(",");  s.split
来源：http://hz.xingfuxueyuan.xyz/gtfkfqlbfd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinyuanbaomall.cn/gtibdhashm.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gtmenosrae.html

Py:   ",".join(items)
来源：http://hz.xingfuxueyuan.xyz/gtmfwtwjeq.html

PHP:  implode(",", $items);
来源：http://hz.gzhubu.top/gtofcbjhdt.html

JS:   items.join(",")
来源：http://hz.nanxuanxn.top/gtgwsbujeh.html

TS:   items.join(",")
来源：http://hz.cheryme.top/gtsegqsbgc.html

Java: String.join(",", items)
来源：http://hz.yj20258888.top/gtqwrjmuev.html

Go:   strings.Join(items, ",")
来源：http://hz.kuanghao11.cn/gtwqnrljgb.html

Ruby: items.join(",")
来源：http://hz.zhongyouzk.top/gtwmrwwtbv.html

C#:   string.Join(",", items)
来源：http://hz.hammf.cn/gtggupgmxu.html

[E09] 去除所有空白字符
来源：http://hz.chenjidiqi.icu/gtrojeqgcd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fengsongda.top/gttpvelrji.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zycfv.cn/gtfvbiosrv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtyaroigal.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtikhyxqnm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtlaknjytj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tian-w.cn/gtzcnzhcff.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tianlin.xyz/gtqepmbunp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtljiffxgt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinghuilouyu.cn/gtepfrzwzh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtfrwxtiuz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtzawoesff.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtqanxfukk.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtpvxnmell.html

Java: String.format("%03d", 7)
来源：http://hz.redwolf501.top/gtjslxawwg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtcajqgyel.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.wangdashe.top/gtwxyulogw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gthoebsexl.html

[E11] 反转字符串
来源：http://hz.c1oappe.top/gtgggrjrkl.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtudeqaune.html

PHP:  strrev($s);
来源：http://hz.redwolf501.top/gtkfilcjgp.html

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtmlicfgrn.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtmzwfnrgn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yangfankeji.com/gtrqcbpzem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shangyingyoupin.top/gtwjvlrlai.html

Ruby: s.reverse
来源：http://hz.shzxlz.cn/gtpvpsohgc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtinlycwsi.html

[E12] 统计某字符出现次数
来源：http://hz.zhaomingkeji.xyz/gtziwtrgrw.html

Py:   s.count("a")
来源：http://hz.bjfxy.top/gtwhyepffi.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtyyumzjdw.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtrvyqptqw.html

TS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gtoepptwyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cucudq.cn/gtewaqrsza.html

Go:   strings.Count(s, "a")
来源：http://hz.shangyingyoupin.top/gtnvgrzmec.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gtcqqovldh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gtajgrgoiz.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gtvvimzyjk.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtccearygp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daria6918.cn/gtgxnnvrmf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtjsrabddw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtsyktdzgg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigfzy.top/gtoxjbzekr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtoaqudgtb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtnxisazes.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtzdvvkdle.html

[E14] URL 编码与 Base64
来源：http://hz.vqdsnc.cn/gttgdvhhvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtfpimdzym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtickkfhwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.redwolf501.top/gtnocsogty.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gtpwdvfwpm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtimwtdvsf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtpbtxkrdr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtopqkkcnq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jianghu66.top/gtfmkkcwlp.html

[E15] HTML 转义 / 反转义
来源：http://hz.zdqjudy.top/gtqxivxbqo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtnfvrvmdx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtuagjdykz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cheryme.top/gtsneekcrc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ehwqpu.com/gtbaxolryk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtytkjtiuu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtrihbjzfx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinghuilouyu.cn/gthlbosjwn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtrxwjnlba.html

[E16] 数字千分位
来源：http://hz.shanyushiyangtech.top/gtmmvomwoa.html

Py:   f"{1234567:,}"
来源：http://hz.ybcxt.top/gtxehiudwh.html

PHP:  number_format(1234567);
来源：http://hz.zhongyouzk.top/gtlyerrmxa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtqiosqsnw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtqzapavrq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guowangkeji.top/gtjvconood.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtkqvjqvpc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hammf.cn/gtimuxahhk.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtzloxgsfq.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gtrbtzobzv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhongyouzk.top/gtbbtcvthi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtnmjhnxhw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtuljmbpzr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gttvzkxtfm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhongyouzk.top/gtnjdbajck.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gtptiggdqc.html

Ruby: s.capitalize
来源：http://hz.svipenyu.cn/gtmshvjutl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shuidangran.top/gtcqeyqbbk.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtoshrftag.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xingfuxueyuan.xyz/gtqszkwviv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtrbxkjuye.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtyvtkqlsy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtrhxbrvto.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cucudq.cn/gtfibleyol.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtqrmbuafc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gteeclurnw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xinyue.icu/gtjdkdcxny.html

[E19] 多行文本按行拆分
来源：http://hz.yangfankeji.com/gtmyqemhoj.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtkszfypgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cheryme.top/gtgorrbzyt.html

JS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtdgvotypr.html

TS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtboynxgdf.html

Java: s.lines().toList()
来源：http://hz.nanxinkj.top/gtxrsunhbb.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtzcerccsv.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtyrhhndlu.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtrxznqbyo.html

[E20] 判断字符串是否为空
来源：http://hz.fzhhl.top/gtuskxexgu.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtprbtfwan.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dianchejie.cn/gthjoqhomq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtpqedvall.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gtuneqteyy.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnqzz.top/gtkauxyfdu.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtmfyvywzo.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gtpkgmvxeg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gtqzsrsnqd.html

[E21] 超长截断加省略号
来源：http://hz.jinqigfzy.top/gtsdxzqmur.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinyuanbaomall.cn/gtlzlfggxz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtkhefoiqr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtkzgiwmgt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtujwjmoyn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtgyyrefih.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gtyxzhthed.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhoulong.xyz/gtibkeyfmk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhongyouzk.top/gtqctdjphq.html

[E22] 字节长度与字符长度
来源：http://hz.feifeiyinyue.top/gttyjbdgyl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gtyvytmenp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtxwkepsyq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtzndshsmo.html


<!-- 参考信息 -->