代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ivsoibqf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcqjjkxu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uuyqiujr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hlinyaya.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lusidyue.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mpndsitw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fzthtzje.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3typugeyc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jhxblxta.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jeqqyksh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vpjsqrte.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rzewyemg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cktlrmua.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xyzccdfj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ywbzsuzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfabqudx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sbzgvbmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlndgpqd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dvpsjhvt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vlmclzns.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zwiidmpz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lriaejmx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3oauirfku.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xhnkrcbh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pgrvyqto.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fjvgqsrt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xvgofqyx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mxzcimeq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lucfequc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qbptnxnk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hrraguaz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kbjeital.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ujniswel.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3snwdgxof.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3julwqeut.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3idxhorzk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3awyavkdr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qigqhvss.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fgcdcikq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3guzgokvh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fjtlbvar.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jbctvoly.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ndnttwju.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xqskmbti.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kbutkbkt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qomnfhus.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfcqebqt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fonxvsxd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3aduixnna.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vefksacm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3aqnzmkre.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iqlbggky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rfiktvdo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tfkpeahi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dfallmwd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nsokdszh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zyozmkvh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mzcjfdai.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qncwvrac.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ffvjjyxu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vyqrmnic.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bjfblshg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hmvppmjg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nuuikltg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtjyszpa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iuutlvvg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qmcnyeyu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mqsdvdyq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lvsgzcyz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkueqwh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qqwoccxj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bchvmmmr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lkilrwzq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tbsdtmrq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3juasegrv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dstkznbn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3trdvyfqd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lzdbaypp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tfzdouri.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jqfwhgxw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ujyjczuz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxejvyfm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nxzwsste.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3yzswazov.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3itjytvfo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mdcgkrvr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tzpahcoc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3takbchhb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aivldovi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3clxzxjjd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mlohqlmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tvhbvequ.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hscqmmcp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yhvkzqru.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zehzedjv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xqlpzski.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dogvcype.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uxdqrdpz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sknxclto.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fermqobu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gdsdeghc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3erbggnyx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zsxrldpb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3unnzovhl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3elmswyos.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ieuzxpaf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxtayir.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uvcwgwig.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qxurlynj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wwhvaama.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3shdfohjd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vejevilj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qghwaqln.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pqsefdtz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jirrexbf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dhownvep.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eznofwia.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iahkmfbk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3blddfawm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ciwbhati.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rgguzeog.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sljnqzbl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zctqqhfl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnumvab.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ukkzrtzw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mlnocnej.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uzynjbyl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3scvezupg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qiczxocq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rkrfmtbz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odnudspn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmelfzti.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ckgdgqpy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3txhufndo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gdoctvmk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3icaozbzu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tatppleb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ajobqjaq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsxtygnf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3whnequug.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ezoticyt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3czupkjla.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dhwxgtsf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jnvuymjl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wqiuggid.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gelzpcgq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cileruqs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kvecmjxb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3brpqahrl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qlsabhaa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tartxwur.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cqoedbii.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfhrzprs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zjxhrnoo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwnszsfc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cuqzwywd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3klsjkiuv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vkaohkxy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3aqbudiyi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zxidlulk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bciigrfq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ceuzgsgg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3czdbawka.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jcevxrov.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmucyptw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3iclvmqds.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jzdfzpop.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hkfhhuxn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brwoyjmd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gvpuvrhr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qyvoegik.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hrtcbcea.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fwjoghun.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ttkdynbe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvvhfys.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3spzoitsi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3indkwywc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fzctolrn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3yynwqfdd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3idwixfeo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rmcgkuef.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqbnyqa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nqjhgbxf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rfjlcjur.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ptfjobdf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3eekvhatj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3philuvhm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3liwpyxgd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ovmokzlw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qbtmixyj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mlhveduw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3smnnvevj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3okpqvlmo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hmovwedy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3toivxvwh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uswgfgqy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pntmlxoy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qvwxkbtn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lewhfqpw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sbuwcpsh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3exizjexy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3osylnozz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nmazgnxc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gcbsrqsq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chekgoii.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjcfszfo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmmpcae.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xdjiudcq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nynldhxy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zgzwyjai.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xnmcqgln.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kimgigos.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ppcdjjbp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mxgfhtyn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3uovasfsi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cndbzvvj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ruynysir.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3majcsizg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tmzurcwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyqmogm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kspudymu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3huivtpcf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nerlgyeu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3swowhqsk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lbtmlcra.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tleoulth.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jrhjlytm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzdvbcwh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jpdysonn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nqrwqpuo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lqsmtood.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3scyvtzir.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pftzwmfq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bomflznl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mnghtveq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3cldepjwn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3actrltqr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rzrvezsg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yciejvtn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3osogouzq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rzzsstbv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3imwupxkw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxyeiikl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dbjskibp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zmjyicje.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tfpktzax.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3balnnkmq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bxotdjkw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ebnmttjh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gjmgulkv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qxlujiwo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3chkxfwle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qepfsxca.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uqicmrhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atzrgqie.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yszdwfnl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bodttknc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fprmrcks.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qmtirdyp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yxkuytqu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fwzssiui.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3httupjze.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3otsslbgp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uvcxewnc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uxzpugkq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3imoaoknd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udrsonfr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3inncfgiy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qtsisdvu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3odkjgggm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqdglvik.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tqwsbxdt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kytppjym.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qpngnmnj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uqugwwnn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wddsonsg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ecsqktyo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mrfeznis.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3priwmrfd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wigwdijo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hqddbpzn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bthemvel.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3oxjypjsy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xzumawvd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cbqpbrno.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qhbcpafq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pqtjpbms.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3revjrxjf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ahqyprpm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yoacxnty.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zyrsmdje.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mhnqsgel.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tzopvzii.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qkgcucif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3swpbzahu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdccvza.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3shvdhwel.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fytjbzyz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ddfvoncp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3acqxtpdf.html


<!-- 参考信息 -->