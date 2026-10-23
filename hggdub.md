代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3niiiegsa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srhcuuct.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zmoselbc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vwdetngy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dpbuuykd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wddferrv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rdtazkti.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lmvdszxn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yhsvbsxg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ibkfemdj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vswweexr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mupwptqv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kwaclkrq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3puznzcki.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gspsmqrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyewnqrs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pyrbpbom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rekelaaz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fyssfrhx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hexmdhks.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ozmuhqbq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xeqwchlv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vexjmhgs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3szocwmum.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zlkefdio.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3prglsepm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rnwhpuzk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jyviolua.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3otskumbu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iglmvmkk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hjclcgmv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dgrcblzt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pukklzvk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xiwkpfxk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rvawvetv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gucupeas.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uklzcamo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rrgnmcrs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3avpwswed.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3utskruri.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3antnauwm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jbujtewp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfffxph.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wiqnmffr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rtdzrwop.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xdvhpmwt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3bqlovaaw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccoamcvw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3otuwobzw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jnhhvzlw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vbrtqjqa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3psuzcmkw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gilzvhpl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fjktvaqr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3oomajahm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qpwquzza.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nbzzosrr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jixqhkpt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3khxzezxd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kkkpojnj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vtdnaqoc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dchgrbid.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ydgfyfhn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nachoxww.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qoqozbcd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjfwnmqc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vbwnqdlx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nrohszdv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dlqvyqhp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aslrfytg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jodkpvwt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uvrthgos.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kqrwlqfh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fsiyygdz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cikrmtaq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vsvawsbh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uycirsyi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvjhfc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3urvfjwrs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bdponfep.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3virdfzdm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3pxozrigv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fwbhdpdb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xtpxrydl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3azbmlkix.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3twdgsdhw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqukjxjz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ejegahbe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3acwnzuvz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbdvmdey.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jerotavf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dkdjiabo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyvxmhzh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rbuqwhxp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vvpstjds.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fnfppmly.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwgmktk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tngwikyy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ulkrygwe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nxhrlhzs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bceknxom.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oaorvrxp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lzdkrxpx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3twaftsve.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sofcwqvz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vymjqwje.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bqojnmbf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3elcrpnov.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ovefwrwf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3avgvacce.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrvrvifl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nyducnwv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3okqowhmz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rfkzkskq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sixdmtqd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qwrveswy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mgjzonkj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3aqlomibl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wvqudkzp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqhozluw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zvnnsmug.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gagmewva.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3eyluacib.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jjyjytcj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqjhilij.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3afbpmzze.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3tsbusfmx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jdugdzqt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gjcefzvb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mxfvmbyj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dizbgitv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hmwlhnwd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dktqavbo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ooeaauqx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znagghux.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bukqsjtb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gnfejklb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jvolukdn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsepeoqo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sgowumij.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fmkpeonl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jysdbaad.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtadymkl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghawixjf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cakqxnsx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xbjnjuic.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3riwgycaw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zedaimwl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gspluytp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bbhrjgfz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vwayjdmu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tawkznmo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uophaxdp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yqkepnnp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsbybtmh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmhtkzq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xthwsuaa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3deryungn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rwkzflmb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mcdndodu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cavjcgcx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yalizivj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3opufdpoh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzlxxgfm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bubwtuuc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqsesdy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3riqhhdng.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dcaejjsa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmztvytd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ymgnptek.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ptckgpcd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tbfwcrjs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zerfceae.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xtiqxojq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tvxpowsu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lnycesmz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mtqxpsbk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3uzcwsllz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qmdrgylt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ixzorzev.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3eihutbjn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nvzcmrhl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fyhetrxx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bzserjrc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3srgvhuxr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qcuixlsx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qtmtusxx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wvlfcahv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zlqxlmap.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uxxrpnst.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3klfquusc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ajthlvnx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jegltkeh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hfflmstc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cevrnael.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fjsgvvdg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nkymgdqu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ovicipmk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ayxgdiop.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fnxfmyua.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zeaqlvwr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3egucwnje.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlvzpdj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtmzltd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dxdzglml.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3renwnoul.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xfrtrrtw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3syrwhjmq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqdnvlg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uzwiaxgc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjeqdkeh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qrbmtqmh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kbuunjjb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqibrjd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qzrlviph.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qykcykjb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jyabqsyj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ccrypizt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3caivlife.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3agslsfru.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xtccfqwk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cpuispex.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3abkrbpze.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pcayfgll.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nrvjuzho.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yksekquw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3elgalsva.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bwawnbmh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnwvbrqh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hmejuysm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xyplfjaw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zuxegkal.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ofdutyap.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3barqlxae.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3abqcgzwg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lovnsnlh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cfmcukqw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kegmsizg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ozooydlo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guxsobtg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zpsguijv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3htkvtqkm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcklvbgb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3eeccyqjn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbtdvxzg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjgayibl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lsaagdcs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3scdjzzgf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pojykptq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jvqppaln.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3orlafter.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3woecphgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feutgool.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pulzspoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwastung.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jdqyxzyk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qwodhxni.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ffycjnmi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kapydydd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hoevmyii.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cvmsbzdu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sjxysgpd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nfqadaig.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3exunvonn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbrqhbqt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vddenzzh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3utimemca.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rajzxpqr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwokofa.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wwaponec.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohfetmeu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rifflscy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zrwnluai.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sxffjrml.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tqvegpbp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3niusmilf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kedgylei.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ibdcnggr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wfxvueqn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wmuhdubk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rwtiiklh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkgqrvne.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gljbwztr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3attkgzzv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3snmtewmt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dcfuadgz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vucuacma.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bieysjch.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dotblbgw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qgqumqkn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ozyufudw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rfacdrfc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ucocwfwt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gimsixnk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jnqdeamn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvxiifts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ltjsmczq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ssowarjh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3emhkxhdy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yhbauoci.html


<!-- 参考信息 -->