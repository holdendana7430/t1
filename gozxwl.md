代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gaohongyu789.top/gtfdpmqkwb.html

Ruby: arr.max;  arr.min
来源：http://hz.hysaishi.cn/gttvhyvotq.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtjvhyfwos.html

[D18] 扁平化嵌套数组
来源：http://hz.ywan-chungtsiang.top/gtawtwujdv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhaomingkeji.xyz/gtomxtzjey.html

PHP:  array_merge(...$nested);
来源：http://hz.zycfv.cn/gtkjlfihar.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gtcxarfahy.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtfpnvcawf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gthbweeooq.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtnjttuinw.html

Ruby: nested.flatten
来源：http://hz.yj20258.top/gtknajqmev.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jqgfzy.top/gtlplaltyh.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtymtgqepb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtbdrihvne.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxuanxn.top/gtenbbcmbx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jlsjyb.cn/gtjkfseogi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtmzjbrssm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hammf.cn/gtkpxqkffo.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gtgckvrqrn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gtfdvfgxuw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenlongwang.top/gtwbprfzly.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtipbwedpw.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gtwfqlrlzp.html

PHP:  array_count_values($arr);
来源：http://hz.yuanzhike.top/gtrpargfxg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtzoyochlr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gttyouhfnc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cashguo.top/gtgfhopeqg.html

Go:   // 手写 map[T]int
来源：http://hz.xuanzx.com/gtuoajzlti.html

Ruby: arr.tally
来源：http://hz.fengsongda.top/gtbvchadyu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.kuanghao11.cn/gtvbcnxpmp.html

[D21] 判断是否包含某元素
来源：http://hz.ybcxt.top/gtegpatokv.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtjrjzlvmu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gtbyleyvhl.html

JS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtkmqekgrq.html

TS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtsudjyfsm.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtlrnaibjn.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtndmrybpb.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtsisdhdri.html

C#:   list.Contains(x)
来源：http://hz.quarkkingdee.top/gtgyxlubwz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangtech.top/gtdzmurxmu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtqpxvugyp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtoaewoamp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aibaodan.cn/gtjrysusgs.html

TS:   [...arr];
来源：http://hz.dashuyun.cn/gtdvdxjiwp.html

Java: new ArrayList<>(list);
来源：http://hz.gzhubu.top/gtlnhdhhcl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhengqikj.top/gttmufuwos.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gtkkvbbovt.html

C#:   new List<int>(list);
来源：http://hz.bjfxy.top/gtdiruemeu.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtfotikbfs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigufen.top/gtqlnrmhvl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgufenzy.top/gtjefomeuo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtnfgxnjbh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtnagdrqat.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtbstqfxsa.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtxyimsdcl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtefvrgnzf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.kuanghao11.cn/gtlfixmxbm.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtoqeachrh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydjk.org.cn/gtzqboenwn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtdexhmovm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhengqikj.top/gtuwryzxut.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gttfvjwsea.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtcdeqmgdi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtkohzsudv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.birdmap.top/gtnmfjqkds.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daxiang520.top/gthlrogrcs.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gtptouczci.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.havefunace.top/gtwqlljbph.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nwbrower.top/gtgxhyvkmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtkddkasar.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangshuangyany.cn/gtssbfbgng.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtfpumukbz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtueotqwux.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sysykeji.top/gtmwfznwcs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jianghu66.top/gtxibcmiwp.html

[D26] 数组转字符串
来源：http://hz.feifeiyinyue.top/gteqgcgaqc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yueranfly.top/gtiaebjjcp.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtlpqzajkj.html

JS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtpfyqtoat.html

TS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtmzywpwnh.html

Java: String.join(", ", list)
来源：http://hz.quarkkingdee.top/gtrmkqmgla.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtlfgfzrkz.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtuujhwiqw.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtwpbbkexd.html

================================================================================
来源：http://hz.zhijiandao.cn/gtstqkqlfr.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtnsgudnun.html

================================================================================
来源：http://hz.ybcxt.top/gtmkdwzehs.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gttohlnahl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tian-w.cn/gtxovelurg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtjcxnwuvp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.svipenyu.cn/gtywibkjxy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtagnoqdea.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fengsongda.top/gtqzdvbrsz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtfnighdoy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gtulwnzuxl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yueranfly.top/gtgmltlueq.html

[E02] 重复字符串
来源：http://hz.yueranfly.top/gtntbyippp.html

Py:   "ab" * 3
来源：http://hz.ppjwa.cn/gtgyobnjgt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtxipvmdvg.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtikxezikr.html

TS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtejcnfnal.html

Java: "ab".repeat(3)
来源：http://hz.52xcode.cn/gtdueknqch.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gtnwxmfjeb.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtrjgkvixf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.birdmap.top/gtmgujhhjk.html

[E03] 截取子串
来源：http://hz.yongpay.top/gtbkwppkdh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sxryk.cn/gtzxsstrug.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtxrczonah.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jianghu66.top/gtlvajlsrk.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gtnvmypwbq.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtwoxvdnwl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhiwuduotai.top/gtzlpxgkop.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtyebefgtj.html

C#:   s.Substring(1, 3)
来源：http://hz.shangyingyoupin.top/gtxexvzwon.html

[E04] 查找子串位置
来源：http://hz.0kj1m.cn/gtaaayphki.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtclymzipm.html

PHP:  strpos($s, "x");
来源：http://hz.birdmap.top/gtaohfxydk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gtsuiyoxir.html

TS:   s.indexOf("x")
来源：http://hz.jqgfzy.top/gtaognenoa.html

Java: s.indexOf("x")
来源：http://hz.guannengcc.top/gthktbynmu.html

Go:   strings.Index(s, "x")
来源：http://hz.gotoacloud.top/gtwnmiijxh.html

Ruby: s.index("x")
来源：http://hz.aizwys.cn/gtobzyzfoz.html

C#:   s.IndexOf("x")
来源：http://hz.yuanzhike.top/gtwvfrlrnm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gtcctyeirs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cheryme.top/gtjmqyurvj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daria6918.cn/gtoevayvmf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gttichixwl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sweek.top/gtzagxcawt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gtgpkmzkoq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258.top/gtluvarftb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtmestqqme.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gtdxjuavgz.html

[E06] 替换子串
来源：http://hz.hywenlv.cn/gtyoppjkil.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gaohongyu789.top/gtkroswaug.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtnnbzmuiy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtqzklraqn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtovcayrtw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtckyfelps.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtjidnpnsp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnqzz.top/gtxlearmoe.html

C#:   s.Replace("a", "b")
来源：http://hz.smart0.xyz/gtrwexmmqf.html

[E07] 按分隔符拆分
来源：http://hz.guowangkeji.top/gtwajmbvnp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nwbrower.top/gtbyxxrspd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtfqzmicxw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtmkiekvah.html

TS:   s.split(",")
来源：http://hz.jyoumei.cn/gtkemwmxoa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ydzc1.top/gtpbmlhjxc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shanyushiyangkeji.top/gtajudhpmo.html

Ruby: s.split(",");  s.split
来源：http://hz.ivvv.top/gtkwqnuwye.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtlywjxvbb.html

[E08] 数组按分隔符合并
来源：http://hz.zhijiandao.cn/gtqtqtbace.html

Py:   ",".join(items)
来源：http://hz.yj20258888.top/gtaydommev.html

PHP:  implode(",", $items);
来源：http://hz.jianghu66.top/gtyyrzypyg.html

JS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtpdwmmfmm.html

TS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtgynjoeye.html

Java: String.join(",", items)
来源：http://hz.fzhhl.top/gtfzoslmgs.html

Go:   strings.Join(items, ",")
来源：http://hz.zhaomingkeji.xyz/gtvlrneemv.html

Ruby: items.join(",")
来源：http://hz.mhx1999.top/gtxglrsdzb.html

C#:   string.Join(",", items)
来源：http://hz.sysykeji.top/gtbpylsvsq.html

[E09] 去除所有空白字符
来源：http://hz.xingfuxueyuan.xyz/gttealxnvt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtmghajjis.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sysykeji.top/gthjtmdzcp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtqycmpxkh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtjkbdxilf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtigcsifoq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hfpthk.cn/gtczosttqb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtnewmkdxf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtvqjnimgg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jlsjyb.cn/gtlorlgifw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xylfe.cn/gtoiccfxgj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnqzz.top/gtwzglxequ.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtrjupdmpv.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtvdjctgjz.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtwbcuyshi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxuanxn.top/gtbxeospoo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtsireqvxq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtzksqqvdo.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtuvzyhozm.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtrrsjpelv.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtzwdwthlc.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtzkazyoyf.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtygdzvady.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtzveecdat.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jianghu66.top/gtcdbyyfxe.html

Ruby: s.reverse
来源：http://hz.jqgfzy.top/gteauqcgzr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtneyjtfsq.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gtnxnksfxo.html

Py:   s.count("a")
来源：http://hz.wangshuangyany.cn/gtabemwcnv.html

PHP:  substr_count($s, "a");
来源：http://hz.ydjk.org.cn/gtcxhllccr.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtcwsxqrhy.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtemkzwzip.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtnicxppml.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtsouaztqq.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gtynlpoumq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sxryk.cn/gtfoimofbo.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtkyidurnq.html

Py:   for ch in s: print(ch)
来源：http://hz.zhaomingkeji.xyz/gttpructmm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cucudq.cn/gtimoqqdxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtkzpbrqlk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtjgxildvu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.0kj1m.cn/gtvrwbqheg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtzxhstbyn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gtzhfnivwp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gthigjahot.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtpbymvskk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtosqxkpow.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangtech.top/gtwpjpnxjc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenjidiqi.icu/gtipoykmyi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yangfankeji.com/gtngouynsu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangkeji.top/gtuiavjjad.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gtqjnkluis.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yonumen.top/gttfgyomer.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gtbdqurcvf.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gtdoszaymh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhengqikj.top/gthawigmrs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtfzjveoks.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtcgmczsfq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtxhyumwuq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtlhvlhurf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtnzekiyfl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtqpcbxrhx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.meibo888.top/gtzymiqtqc.html

[E16] 数字千分位
来源：http://hz.hnqzz.top/gtfkuqkxpn.html

Py:   f"{1234567:,}"
来源：http://hz.316326.xyz/gtkjeipbcq.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtnuevfpab.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtcxyxbfjq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zdqjudy.top/gtrdzvvzma.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtbvtkcnvh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtrbhfnurx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ybcxt.top/gthbakmowj.html

C#:   1234567.ToString("N0")
来源：http://hz.jinyuanbaomall.cn/gtbogqfbkz.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtvethevih.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtbxqkhkza.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gtsmczllgl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtomgktzyr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gtbvhrzsnx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhixingplan.top/gtkpnidmft.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gtfnegpbit.html

Ruby: s.capitalize
来源：http://hz.yuxming.cn/gtzaepdcqd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zycfv.cn/gteeuwfpnw.html

[E18] 模板占位符替换
来源：http://hz.tanke756.top/gtoopsegqh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtlaucvhdx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtqxiawzek.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtnxqhvuso.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtyaaukxqc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nwbrower.top/gtnuugmhdr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuanzx.com/gtopzajzgr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cqqwz.cn/gtpbewxvqc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtjricpecc.html

[E19] 多行文本按行拆分
来源：http://hz.yangfankeji.com/gtykmbsbwy.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtinrhjjov.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gtwkhijhnb.html

JS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtncjisrxb.html

TS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtfoljfjwt.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtlzvpxojr.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhoulong.xyz/gtajydhlsm.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtbjzogudi.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtfzbrwras.html

[E20] 判断字符串是否为空
来源：http://hz.aizwys.cn/gtlmlwfpjw.html

Py:   if not s:
来源：http://hz.guannengcc.top/gtdcaledgm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtjvthlpvx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtimwkmesm.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtaufncnho.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigufen.top/gtfraymwpt.html

Go:   if s == "" {}
来源：http://hz.hnxiangtu.top/gtvknyhqux.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtxhuoubjw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtmsbqrkpz.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtdppoocvk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hongshengwenyu.top/gtjdxonvvh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gtstzpyivf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtkirsqqcm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gthfgkljbw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtjoirjzjo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zdqjudy.top/gtmlreeidn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9152youxi.cn/gtdsunpnnv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtqfetlaci.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtezmdywcu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gtcrmsdgcp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtuqnuphvj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtvwkftcwr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtlhhpxqfx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shuidangran.top/gtfhiptjzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtqyykqyia.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangtech.top/gtmblodyej.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtfmnzohsu.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuemavptx.html

F. 文件与目录
来源：http://hz.ivvv.top/gtnxwaqswu.html

================================================================================
来源：http://hz.gzhubu.top/gtfqqeimkr.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtmqjwplcs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhixingplan.top/gttxnahxmm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.havefunace.top/gtbnojogbn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtdtrguuev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtbbgdjrvd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtdjcifkor.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nwbrower.top/gttbnpwydr.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gtedsygowz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtideyyfqt.html

[F02] 逐行读取文件
来源：http://hz.yj202588.top/gtzwjawrjk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daria6918.cn/gtmxeygozf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zdqjudy.top/gtzizmtipp.html


<!-- 参考信息 -->