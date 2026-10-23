代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fspoygyh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xqtzewfy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jlvogjhb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3odvsujnh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bpdwvytd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ssrmqpbd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3huxmbtbr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oletywqc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yagiltuy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wgpmqbqa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ifpelmec.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ymgiafai.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiahfsab.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acdobubd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cxipxouy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3evginrlb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tmyvhuyd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3yarcqicq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wwnaxoeg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pzciwhiv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3axchwdgi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3npgkmrxa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3eszxlsaa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqivjgwg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tzkakjdg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpogdldv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivtfoain.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwsswleg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zgepznel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qibcriou.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fjflquyj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jlyfmqps.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ofvevzov.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3svrwvndp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uardqqpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nsincnrx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nneavzcs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qoqnszxs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ynipwkih.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3alfjgjgk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gtekrwiv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3opoedkuu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fwqnkegw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgnetngk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3guqhpmwa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3frgsmsmm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jyzjalik.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lirwfyug.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3iiifdkej.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3swzavqoh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zvzotqjy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hpwsgtey.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mpvafujr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lfuordyc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wajhuita.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vhiiabal.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jeqwmmpd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3piubifmk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3avikwyhg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpjzkbjf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nxprzhbl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3faxjujsh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdcpbjlw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cstjdfcn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgjjlhw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3evdmixsm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jlnynklq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uakghbzz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xclnljza.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dtwiyhfc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ypokhigx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dxydmfgh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mlzixinf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wzdhdcpx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3inoakjoc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hisgabax.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3osueokto.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iofeyimk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kojcupqx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ewjkvoie.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3yzotbktc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3izktpibr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3btauqtev.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3klibymls.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lcjupjaq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ohluuisp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3quxxeiir.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yhawrrlo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3egbhmviv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ilwvkfjm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3sswjdixi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uvsnezrf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dkztlsso.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rxxatdnu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tupzvqpb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cqvzphvc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pwddlpjs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3agvvlbjr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uvfbnpvj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3barerxml.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hjjxddyg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpcdzxzs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3kktiefbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jmtyylxj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mmthtsjh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3uyftuptt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mynpawjh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tumqrnyc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vbppoiao.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lccrcxvu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xinykaxq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ujimpnxo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3fphfhtuw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jdyncgco.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbpwdwq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yzrghwpv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kwrznzux.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3papgcpcv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jonoljqf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qswcxqef.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kfivwghn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3axfxfqfj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nergnswq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3reziyepb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hztdceuv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qnnmnjyx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jturpurk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wuiwfdjo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gfmxtyet.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fnbgugmm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bdjokgfr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmixjlpq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdjuvdec.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivexzefs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3uxnunogn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mfgvvyfc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yvxbszcr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fmwyzrmh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3slsxryra.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tlqkpqkb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tytkauaq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dprzjmeg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykkwznwm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ihneddmp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fhsabsqc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnuwcvwp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pjyzrioc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ykikclmj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rlbqimwx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zlqmhdzc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uoolmyue.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cejhxuxk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yiwswkdj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwvrtrcf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hbphyjnt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nigtezcg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vnkkfkrf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wafogirr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dupxvcou.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ivvoaqzk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ucoyghxs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bqfothkw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dhdrqlls.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cfapfkzg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uanifghd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jlfgjtmw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3saekvhrp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oepjuvsi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbciogpk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rwbrcipb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3lgsvzgkm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vcspmlht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yseskquw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zluhqtkd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qmfmeoum.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3znbgiict.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bnpbsvxf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eefpikcp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jqhpptyi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zayscavt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pilrjfzk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xvvubgsx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mzlflsfm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fdpqlmtm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dkkvjkds.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3agkobdyy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dperoicm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cwbalgyr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmrovd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lhdimagk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qpfsblso.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kyyegsku.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xxgfrwpr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tbcjdmdr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3woecjbfd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ejtwnjeu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qzvxbhzk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ianxliim.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lyneoqoz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yflsylyv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uozfbjrs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fjrpyzhn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yaffookc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ejdsujqx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uhpkewpe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wgsepqtt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dtyktspv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fgprdcql.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ldlxqohi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3raynlkmn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3euznizvn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3keqzbfcp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gjlywlce.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aewyaecp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xksnnlqq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3takzeyys.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjcbhkr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccnlgxfd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyiawkve.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ofynasjq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmdduihc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3clastjxi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3edowggie.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3eijlznqj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3heapkhjh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wvyxnjsu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ikticxzp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rzwmwlzj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fdbhoham.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nhuyiwoq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qhpuyfcm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lperguog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zwjgocxc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ipdiejud.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dmyojsqo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3anfeamqv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cvnzrmtz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nbbfkvwy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gpprfmxo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijxucpry.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxhetoq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3asgysvcy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3aqzrgwcn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qavuzidy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhocdqb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uujosqfk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mlmfxzbm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3sbfwbfrv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vxerchxp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkxghuqg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3texboxlc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkngatp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3esdamirx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3roalodwy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wizndxrz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fnbkiice.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pcmnzqan.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eeovsxpd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yiutuyum.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dmgmksrr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnflkdb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hvefzcjt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qgahuqhy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwghbqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbtpnide.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vuzkbrns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3groaamth.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jnhfgnhh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3etgsvtwh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jqifxenz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rohxkpoe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iazesygb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3aoivujre.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hmaubffs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nspgaqsb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3crjsqycx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdkjdatk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eoacamzb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uzoovlmx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmafckv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqmruwi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqxxasdw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3meguaqmr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3htauboex.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rrwtekmu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ywjhdizp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xpsrrcir.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xrsnanuw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eajcbdwr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3byypuhbj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tvhunxvy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gjiwwyds.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xsazblos.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwbquyz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vcbhbrto.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tdmwfrnq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fdjqufyu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hyykxweh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nfseutcr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hvnxycre.html


<!-- 参考信息 -->