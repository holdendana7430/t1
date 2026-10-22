代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2znrxegdc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ihqzonfc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jrlmzuif.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bpgnxaka.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rrdstcfv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rvqgpqnn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2phjgfrzq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2abcvzasc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lwygjomu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2adkjmmbm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kxgqvmgy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wgalddui.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xizpdzdo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2csutmkfo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sdbcevvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdfhonin.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pibfszhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pntcntgw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dsxfifpb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wxpybpet.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ivlhsxes.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yzqomgwe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wxpboncw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ywqnjlwt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pjdozoes.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cceumzyg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2npcfdasw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nxifdrtc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lopwrnga.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2sfuaxdux.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xzqntnzs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2opuxjuws.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fuohpxut.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjtouat.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbeenhi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2znlxlyvq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hvfydtig.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cffkzjgb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cuedcyss.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ktqoqvnf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2epcihciw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mgbnirsd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cjvluwhr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjxlsh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xuvfkdpy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tqwojygl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2daxgtzvu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yclhhqxp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2frjqrxij.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2snteausk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tckckaqh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xaoinods.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dwthnmku.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zwaxxpfw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xhtbtova.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2btkgnsxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yfsnixog.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sbcvqpzh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2msnglvik.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2owblykdl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kpdsczaw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xwvgeeyq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ocbnrkhe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2urtksohq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqxspofu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zrsopngr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dgmiixjw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qgewiszl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rtrwkpap.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqldsqcs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pkcxckcx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dvwvrkkp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nqfdmfgc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xlxvbqen.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hehcmapo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iqewvzju.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eugjialr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pkegzkes.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ddtarjep.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zhwcafyc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pbjpmoor.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jysbbkqx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jtoyzzkp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2doiiqytw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sopbdwsy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dvmyetuy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ubaswdrz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dkroexyq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2angcgcrb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2htdlhzkc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nekdvfdk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ufikjekq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdtmfkhj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2iqeycvwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wbaqarku.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ickfquir.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttdldogy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mwezqbdz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2stzgxqts.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2dgimezcl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zsshttad.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bfpgxwru.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rvmblbdy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fimhbnon.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hvcykzpz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vparfnuh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xtlcirbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kesqfrns.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pakhovps.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2syyqklbp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2sqixyfzq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cmymjrlk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iizblzya.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vlyntsvl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tyayoeet.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yzxksdzs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2whfyefyg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uwskqixl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2covuxbyl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mctpoczl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hznpfpae.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hxeosqrp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nddiscec.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yymbrexf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zwxjzsze.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hygssned.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ohuxjxmx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hcvchbfc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ywcsvplc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhhrhks.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtbdtuw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwkmmont.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pcnnyfum.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqfeepav.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hvmrbcnk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nqbullit.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2octgbgdj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwfjfayr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2luatoewo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pmuwdduy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tndfgams.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2drylsiqc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xebaodin.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sytcpkbw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pytmrknq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fkvezyqz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2awdymyzv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eoilzdkl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hklnzaji.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mxgfhhwv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kixlbblp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2umnbhsga.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yvkearza.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lwrrtkcp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qejupgah.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvbrxrd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ynxqsszl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ggwayvur.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mrmqzaly.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zfvmozgb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vgcmjtiw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fdggtlae.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2thdpfyjg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bablwbxr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xobqhvne.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dygqvzhb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nzipnrlg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2efwtwdzx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhptfkw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2lrqgfmjn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cfitomao.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2sqytbloi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lduizvxq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2stziamiw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzkwsol.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zgvjdvbm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ifyygtpn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fammbihm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mexppzvg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbwwfull.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2enqgmqbc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ucnuwqad.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2akjiwsre.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sbteovmx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2olxzxtck.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2joqsuuys.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tognbyhc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2epagdpvu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dxabhgvc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sqgspjry.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxectvih.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2remmhhnp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zfiqvwnj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ueretqna.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sqyaiifc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kaxbxoin.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nsrgxulx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2beipkayc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gteeuwyq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ryjunwxb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vtufiwpe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzocergg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qgvisymg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2axtzxqak.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bxcmskiy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aacheciq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqazecvk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lvoqbzos.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbywwevf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2myvdubcj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nilavpjk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oxsoarco.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2efbpbosm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2umbmijbt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uqglxino.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2polegjqa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bksriexh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dyalofgd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mvbkodsu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2maknxkjt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eictpyuj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2agxerokb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vgctnyow.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lxtzqdcm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtawuumn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mbfwefxz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fzgazqjf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpemjhnc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hohywdwp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jahkojum.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2atltdqrb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vydwtzur.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vjaedzem.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ztjqrxnt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2smwfufoz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bznomhuu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yozpvrjd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2khxxduwf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2knphfmnr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpriqnpu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nctmxxru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuerqcjm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mlcueoed.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qntncfyy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cramrcux.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jnzunlhm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vqywdicc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2offjeyqo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pdctrmcz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2puesncbi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2htyipuin.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nigcspkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zezyhpyx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bkapyesy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbwrgfqt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzqtkikp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qveulmkg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bsfjysrq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kggetrtc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eiedobpw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycvtlzjz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tgmimlrh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2egttcdlq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdppwmvl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zowknycr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sfdehhud.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xukwmjfl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tolbhbjm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yzbauytb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iauttoki.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxvmfptq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tcydyftp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vmlfgudj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ewdgxcaz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mgalupfl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tkjcjffp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bfaubxlu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvpdylsz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zvyzhnss.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nktbuous.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xfpehhdt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdorcggj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dsnrbeee.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xctcwrwu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rwvroknb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wlevoibw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cqsjjtry.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2omtankgs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rzivqsua.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tbhdhlky.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lkatvyht.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hdwaqjrz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2swhfsogd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vbxuubkj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2khlrnhmz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yhplgdzn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kxvtruvq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ktpgepfz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zlqlmrqx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gzqreyek.html


<!-- 参考信息 -->