代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yueranfly.top/gtrjwdwhgw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtfbdyjdqt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtiwgugurx.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtdpbgzqtj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtojsuvxtp.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtqvbicmlz.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtqktgfvef.html

Py:   max(arr);  min(arr)
来源：http://hz.tian-w.cn/gtgrnxekms.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinyuanbaomall.cn/gtjofwdigx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yvedp.cn/gtcioztgru.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gtnkmwzmwg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hfpthk.cn/gtfesccqgd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtkbocmeup.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtlkncqckb.html

C#:   list.Max();  list.Min()
来源：http://hz.hysaishi.cn/gtlmlavjzo.html

[D18] 扁平化嵌套数组
来源：http://hz.52xcode.cn/gtpqcgxyvq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.bjfxy.top/gtvcpktenp.html

PHP:  array_merge(...$nested);
来源：http://hz.yanxiufei.cn/gtustsvpzi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtujrmbscr.html

TS:   nested.flat();
来源：http://hz.daxiang520.top/gtebksnjvb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtibcoxyjd.html

Go:   // 手写双层循环
来源：http://hz.iojbl.cn/gtjawutgiq.html

Ruby: nested.flatten
来源：http://hz.xziqi.cn/gtvppsjlbb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinyuanbaomall.cn/gtiqtqqyie.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtrvplqyvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ybcxt.top/gtsiyiwmoa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangdashe.top/gtvgxjhhgc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tianlin.xyz/gthtlqozlx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gttgenzxcn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenjidiqi.icu/gtrmjyfzex.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtwihqmeso.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtjxgmhkco.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtwsiqfygr.html

[D20] 统计每个元素出现次数
来源：http://hz.cdnleiting.top/gtgfxqfmbw.html

Py:   Counter(arr)
来源：http://hz.ydzc1.top/gtuujybazn.html

PHP:  array_count_values($arr);
来源：http://hz.xziqi.cn/gtqrhsqhwj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtguhrjycl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtukfnaycs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sufxvd.cn/gtyorxotrr.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gtmwxyxefx.html

Ruby: arr.tally
来源：http://hz.daxiang520.top/gtnefaswgz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtginhstnh.html

[D21] 判断是否包含某元素
来源：http://hz.cashguo.top/gtxxlnhukd.html

Py:   x in arr
来源：http://hz.dashuyun.cn/gtjogtdrou.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxuanxn.top/gtskcpqkzw.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gttacdeqsv.html

TS:   arr.includes(x)
来源：http://hz.zdqjudy.top/gtdlhdalkn.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtwirexzxo.html

Go:   slices.Contains(arr, x)
来源：http://hz.pycfn.com/gtcwoozaip.html

Ruby: arr.include?(x)
来源：http://hz.mhx1999.top/gtvlobphtu.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gtrznkazuq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.birdmap.top/gtgvrkieon.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pengpengdd.cyou/gtjephabxh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtfvnwpbtw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtgstrlotl.html

TS:   [...arr];
来源：http://hz.wangshuangyany.cn/gtriepxvnu.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gtblagsicd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ybcxt.top/gtwzdbkfma.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuxming.cn/gtunftofkm.html

C#:   new List<int>(list);
来源：http://hz.yuxming.cn/gtmtsloyfm.html

[D23] reduce 累积计算
来源：http://hz.c1oappe.top/gtlmxwbkkv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gtudnadkdd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtkznxuoby.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtjbstpmba.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtuxwurjpx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gtiuclsxxn.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtzywcrsad.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.birdmap.top/gtisohjydo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtyiactcgv.html

[D24] 字典 / Map 基本操作
来源：http://hz.tian-w.cn/gtudcbbaeg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gttpieywkg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aizwys.cn/gtorqdjyjf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shzxlz.cn/gtaorubqpo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuanzhike.top/gttbybrbsb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nwbrower.top/gtetmkzkzg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.aizwys.cn/gtrnzdtigo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgufenzy.top/gttxdgidpx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yongpay.top/gttzxaicfm.html

[D25] Set 集合去重与交并差
来源：http://hz.pengpengdd.cyou/gtgnxyfysy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.aibaodan.cn/gtwdbpjekl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sweek.top/gtgujquhlg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtdtgyyksi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtwvzkfczr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtvdoinalv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gtsizaddja.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gtuythzulq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sweek.top/gtapboatjv.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtkjjzbmxl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtwtqqloix.html

PHP:  implode(", ", $arr);
来源：http://hz.redwolf501.top/gtihooyqjh.html

JS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtmhhpcsxz.html

TS:   arr.join(", ")
来源：http://hz.xuanzx.com/gtibibyxbo.html

Java: String.join(", ", list)
来源：http://hz.chenjidiqi.icu/gtfxvxktel.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtdppydcvj.html

Ruby: arr.join(", ")
来源：http://hz.jinqigufen.top/gtcjqbzrmy.html

C#:   string.Join(", ", list)
来源：http://hz.guowangkeji.top/gtujamopvr.html

================================================================================
来源：http://hz.wangdashe.top/gtompiqqxw.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gtziqnyhtx.html

================================================================================
来源：http://hz.hnqzz.top/gtmpqrjlzi.html

[E01] 拼接字符串
来源：http://hz.jiagoushi.top/gtqoczyzzh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtzehrjwzb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guannengcc.top/gteaujimco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtbguacesh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gthdxuglop.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gtolntzgbu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinyuanbaomall.cn/gtcoajqqjh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gttmrdtdjr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtxuzgspmp.html

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtcaioewao.html

Py:   "ab" * 3
来源：http://hz.svipenyu.cn/gtrqslqlre.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtkleszovl.html

JS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtcblvwgqz.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtempdlpfn.html

Java: "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gttvhztbqx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtzkfipdfl.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtimbbaymc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtsamhloxb.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtsluanocv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtzfxvctmh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtmysnpubk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtjubedcoi.html

TS:   s.slice(1, 4)
来源：http://hz.cheryme.top/gtcszkjloj.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtyowebziy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gtbfxzmgfi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj202588.top/gtkjamsmmt.html

C#:   s.Substring(1, 3)
来源：http://hz.ybcxt.top/gtmnbdkivc.html

[E04] 查找子串位置
来源：http://hz.wangdashe.top/gtvwermkaa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtufztzpwk.html

PHP:  strpos($s, "x");
来源：http://hz.zhengqikj.top/gtitvdllmj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtsebupyfs.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gtvzbdpuhl.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtafhumyyy.html

Go:   strings.Index(s, "x")
来源：http://hz.ydjk.org.cn/gtbdpntauh.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gtaaojjxta.html

C#:   s.IndexOf("x")
来源：http://hz.xuanzx.com/gtjqjjzdwx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258.top/gtbrbuqdbf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.0kj1m.cn/gtpekslpai.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinyuanbaomall.cn/gtiywurjlx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.havefunace.top/gtfiandwwz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgufenzy.top/gtejbvyaxb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtvigfwxpd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aizwys.cn/gthdmoymgg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtokqjtbff.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zycfv.cn/gtllqqrrpi.html

[E06] 替换子串
来源：http://hz.redwolf501.top/gtmloyyzqy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtptprxyuf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pycfn.com/gtxcmbuvro.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtbktjalff.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtkbwcsybw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gthmrpesnm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtofuwjhyp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.kuanghao11.cn/gtxyczwxzt.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgfzy.top/gtbdsuveje.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gtogjzsquc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dashuyun.cn/gthkibweec.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuanzhike.top/gtkjgoldix.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hongshengwenyu.top/gtykmyhmyx.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtqnqbnhol.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sysykeji.top/gtznlorvyh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhiwuduotai.top/gtyqrmclyv.html

Ruby: s.split(",");  s.split
来源：http://hz.xuetiantiany.cn/gtjgxuzlpp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xziqi.cn/gtsmiygweo.html

[E08] 数组按分隔符合并
来源：http://hz.gzhubu.top/gtyaawkutc.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtbodtjaaz.html

PHP:  implode(",", $items);
来源：http://hz.gaohongyu789.top/gtnsxtmtqt.html

JS:   items.join(",")
来源：http://hz.yueranfly.top/gtumtinnzk.html

TS:   items.join(",")
来源：http://hz.kuanghao11.cn/gthgequbny.html

Java: String.join(",", items)
来源：http://hz.tian-w.cn/gtebqvdhvk.html

Go:   strings.Join(items, ",")
来源：http://hz.iojbl.cn/gtpdlupfaq.html

Ruby: items.join(",")
来源：http://hz.andypj.xyz/gtfiviuizz.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gtiucwkmrv.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtxmnexrps.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yonumen.top/gtdomdlbjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xingfuxueyuan.xyz/gtvzqadnko.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gthebplfit.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gthslqyrpp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtaktjesbx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.iojbl.cn/gtlkqiroxw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtqcqcxvdz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydjk.org.cn/gtrqilehjv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtqaclprah.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sysykeji.top/gtuyfkcgpn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtoeyzbypr.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtjfpdmtiv.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtooxtjqze.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gtxjyuxjno.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yonumen.top/gtipgxunue.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtrmgiewjf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yuanzhike.top/gtnowxdomn.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtmqetuedq.html

Py:   s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtjjmktyit.html

PHP:  strrev($s);
来源：http://hz.c1oappe.top/gtsafxsyyi.html

JS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtroiwbwcj.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtneirjgdb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yvedp.cn/gtddustixp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtnrxhvpoc.html

Ruby: s.reverse
来源：http://hz.shanyushiyangkeji.top/gtrwazdgdx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtwakpjyyv.html

[E12] 统计某字符出现次数
来源：http://hz.guowangkeji.top/gtopdzqdep.html

Py:   s.count("a")
来源：http://hz.dianchejie.cn/gtaismsaei.html

PHP:  substr_count($s, "a");
来源：http://hz.jinyuanbaomall.cn/gtwiexgmji.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtslzbxbjr.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtdwodizbv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtyusjcxbd.html

Go:   strings.Count(s, "a")
来源：http://hz.yvedp.cn/gtaknanleq.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gteqioukxr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zdqjudy.top/gtbaktvuam.html

[E13] 逐字符遍历
来源：http://hz.jinqigfzy.top/gtnvgnxcbf.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtlohajojr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yanxiufei.cn/gtskxusjrw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtuhdoxyot.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtltcrwmzh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.mhx1999.top/gtcndacnwl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hfpthk.cn/gtnmvhmmdc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cheryme.top/gtmstcojvs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtmrjoykbv.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtwnfdahlm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtguvmlfph.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtjvrsbdvy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daria6918.cn/gthreyvwxa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hfpthk.cn/gtnyxcadhn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtqyfeclvu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.havefunace.top/gtshrwckui.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenzaomai.com/gttrolwrve.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtpanhiarg.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtfrzfibji.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gtysykdqbe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtdpkgqgps.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhixingplan.top/gtkrptflmj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.feifeiyinyue.top/gtevrbnedm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangshuangyany.cn/gtnpxqvlje.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtdvcgmyfz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.quarkkingdee.top/gtbbtdzfwf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtcrfvadrk.html

[E16] 数字千分位
来源：http://hz.fengsongda.top/gtpewmqbon.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gttwxxnrzl.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtucjejeuf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtvuhsdgln.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtqlcltcwb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sxryk.cn/gtwytefyty.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtgbkuhriv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtlnasoist.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtpwrnziuh.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtjijsvnph.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhoulong.xyz/gtbcelggqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.meibo888.top/gtzopwqjzf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtdupurltk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtsxakdmjz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtvefwbeph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.316326.xyz/gtyvfpkxov.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gtletkxowb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.bjfxy.top/gtsybmgcmd.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gtsdiptbms.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtelgdgbaa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fzhhl.top/gtrmaklajx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtjnmfjtie.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtavwndkua.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.birdmap.top/gtpmfzxmuc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hysaishi.cn/gtewnunuzn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fzhhl.top/gtjqzimhrh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtbzscwbqz.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtmagbgwye.html

Py:   s.splitlines()
来源：http://hz.yonumen.top/gtdnwygvft.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtdhkwvfft.html

JS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtdhgugbcv.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtxeltaluo.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtwhiljmlv.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenjidiqi.icu/gtnpjpnurp.html

Ruby: s.lines
来源：http://hz.guowangkeji.top/gtofskhxre.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gtgdefodov.html

[E20] 判断字符串是否为空
来源：http://hz.xuanzx.com/gtzkfpxzer.html

Py:   if not s:
来源：http://hz.hfpthk.cn/gtjjdxtujl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnqzz.top/gtcpmhpdch.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhengqikj.top/gttamibdvu.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtbtoichaq.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gtlnvxckrk.html

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtfbyiinpr.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtenlvedxp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258.top/gtvwomgxxl.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gtcwtrllyp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guannengcc.top/gtfvtxptin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gtfmjlnjuf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtmwmrzhyw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gthynsaujh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtdszcxxwq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtknypitwq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhixingplan.top/gtwijqybgb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtivltdujx.html

[E22] 字节长度与字符长度
来源：http://hz.ydzc1.top/gtxfduegnq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ivvv.top/gtjghkxjcu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtuturhonu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtuhjyqsvo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtmvhqzwcx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtggephrpy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtrhvaiulv.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtigepnqsg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ybcxt.top/gtrcvixwlq.html

================================================================================
来源：http://hz.ppjwa.cn/gtjcblmnjm.html

F. 文件与目录
来源：http://hz.havefunace.top/gtjjhiysmq.html

================================================================================
来源：http://hz.andypj.xyz/gtghjhiqji.html


<!-- 参考信息 -->