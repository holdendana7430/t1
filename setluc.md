代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ncxijevd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2siwrjmuw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xbhfbsyu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwweglkr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igmrjmjl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gxmsbguu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2iubxhsig.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sfyorery.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqejhchw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zmbwksvm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2willpewt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ehphrpie.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpxdhnin.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bjlhwpuf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yrhgeudx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2awmuejgs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2voufhxru.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2oacilfql.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iokamxfx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hfaprvhp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2apyfycvz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2acbjuvql.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jvsosknb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ztpjkith.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fjqxotwa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cpivnprx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tyxtuctt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uxbijcki.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tclpshxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjivrv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2etjtypby.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qjrczhaz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2agmjiujz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kmwpnbxx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtezgbgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcixcbgt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ofwybubf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlmaculh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dzeaywxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rjktnoks.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cozlmdop.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bnxvkimr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wjcqthsf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wtesgjjv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gedmrxsm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wnwvespl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wxsvdxnk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fgjguqaf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fnugdzhr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2whtgpldb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysorfqxl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2aatevhjo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2msrednfo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jobygczp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ojdzzifs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmrhcmzx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mgprtuut.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rozjgghh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nggrahnl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rxhnwdbg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sjavnino.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wzuoziti.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ixiijavu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dwrbfnqi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2drrqnhkj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yymdvclv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zlhywjkv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hwpjxdwz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2efttyecg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jeawzskd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tjcpfyfw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kantwewx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmusqkzb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pnkrivpj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2knwpwaef.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aetuscuh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qxbgarks.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tdbgvped.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2esdzzcvf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ihxlpdii.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yoowmylq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2spcphiwg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qqsxjwza.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ydrcxlwy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxnzips.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xspzfcsk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kbnsreov.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qpqugrnl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qjdmyhek.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kddoyrkq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cdzskyag.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2flctoupg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dssgvpff.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qzuvktev.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yuypukpm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tvbianch.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2relcmcln.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xbbjihju.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wwwivqve.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2upxahnfs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvvekcju.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wvjlvyhr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mipoymia.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ngziaevf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ybaufxrp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dgafpvew.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2utwikzxq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fouzkcwb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hfrqeuyl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rxdpmztb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tqvsrjpo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rgnvsiak.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxegkurr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zcpruaei.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kjmzcpdk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gascfhzo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ahojuztk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qhwoiiss.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oywkmedw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2sceijscv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfznluk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lkbfejqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pzyajibt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pmxhillp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wnvbvnyx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lmalcdiv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lrdnmmww.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rnkgbmvk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bmbvtyws.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pcueupqa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ryuqbdgq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rggakxbs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xgdzwdhd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zjspmzdz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjgzwxfn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2iswmvyno.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wgmfotaq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hmiasaer.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cgmagfvm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfhpsvpq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2plqkyklr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vlaoogci.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vylfjqug.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2legdavcp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrttelk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2obfzcsqz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gvcmcnkr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pobqsyut.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vymdesfj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2orhhkofc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xwjxglrs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfqwrmsd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tculphbu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2eecrqcdc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zxtvcper.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2npxsrshc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2sgewngxt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zpfuafst.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2arlptnfl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmkhgta.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvfqnuzm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2manabrnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsmsexhq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2klvanjuz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2omasbmpm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bayqyihf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hocicbmb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tpijvisy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gyigepfg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2keaselpb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kfytnyvg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tpnpppha.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ooypveti.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mtxxsdiu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yixaxwpu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yliezwxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ibtwgdso.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xbulwscw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ahusighq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2iwnxsewq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bpddunwg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mcvkjdmt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bpzfhtaz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ssmrhqvv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rurrisjj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jpxrtxza.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2leaccedr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vksulknu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfzsvubl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2lwqzphdg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2amveutty.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kxvlsray.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hxkmozbi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2icflafjt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2imlalrpl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dzuylzle.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yxsvwvzy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zztrpjin.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cyekxyeg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xyodguzp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fxrudmfk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gzlubuoj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2aokfrftv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dtxuabix.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yxcdntjb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vwhkuhwo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zhigjgnb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqzefoe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bvmgbwof.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bkcvcodc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzaansx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iugpmevt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fexdwopt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uyfzeopu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2woniiibi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2adkzgsyo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qlnlgxff.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qunxlvmp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yfpvcdsx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ljrtwbut.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zugtdzzu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ecymndtu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2febzklqi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rhtveheq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wtcmdtie.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjmpbcy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ngetcpjn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ixjtaicg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iklonijp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wxepbbiw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qcoqgncl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cdsexmrp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tbosrguv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2phckikiw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vmtuwcay.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ehfbtrtv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2opqlgzvr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yllplafc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2avbftotc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2klptjklw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2aywwmulw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2alzwdxws.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwxddxjz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2trdxvhnf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2puiatcdm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wnqmabvo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yosabtcu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ebreyvid.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2piibgwel.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uindhriq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2acnwrqie.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gauziffx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xvfdwgey.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ofqzhach.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fcqoehfa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2udsoxazi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vabitwhk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dkouqwtg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lyromzam.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwelhjfl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vosuhues.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2emkocizc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmxxvapu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2obcqbkey.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zkajmimn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sfpwczfa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ylnotnog.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2btxxnyqc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2abiopchz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mjdvevkv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wutxnxpj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wtmoowdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oojglobn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nkjjgtzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkvyztkj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwnczggf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qzawctni.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uygskrda.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fayquuzp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ujgtkvee.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yeqizzyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tolidttc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bqlhcypr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qmbezoxp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytgpxcrx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2snozzihy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kdnglwgr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrptqbzc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iloivoqu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lchzsimu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yjctbkcq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uilznveg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gpjkxled.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vhwecchw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2irrnwaah.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gcxgxwip.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hivfbjlf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2heaqfljw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dygnrhos.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uzojvjss.html


<!-- 参考信息 -->