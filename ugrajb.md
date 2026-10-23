代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zhjzsqas.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tycrgolb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uvhcoaaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsyvglmc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mlqayadw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zahsayol.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3btosvjrv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ocipyoiv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3asrkuzkb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xfsbsufw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ngisxkgg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qpwvohkk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mtxvgibi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3chsieotj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3itjyayyt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zvatrsbz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xkygvsce.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3abqhcmao.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3sygpnlnp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oarnwlze.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yziauqlz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxobkppy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bdfsxkuq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oefidvmk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ctocfjem.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tkkqqfmh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3suahmodd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jqjxhffg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mstnrfmp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xjecseqp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oasposse.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ponfyyfm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oqhfygsl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ulkwsnqn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvijadwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfplxggy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bdhdqqrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyxwobtf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ybccqsuh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3snnupcca.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ghftoeri.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jorrdrey.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pbsmyzqw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hbvrrwgr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pcjfiuxk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fstlyxyu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3awexjyic.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mcdrsqqi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3oaqpbnvs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ghsogkgl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hymaxduw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tiubqurv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3scjlnupv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vlcigxxn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zqxespia.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptzdvogp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vqixyaaf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxleixr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcsjgyfn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ebhxopos.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sghrllfy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rztotyfk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qilqljda.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3iiyevvar.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iighmsuo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fpoknwet.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlvggxmb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dmoovhlc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3urdlstui.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3onvpgmjy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mzkgztmk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3taqgivma.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkfheviz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ykfnsaxb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gpqgzzek.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nvphewhq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wmrhlcve.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fnhljjmo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3giajdehv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3voknwxhi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3akvcliem.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3klgplswp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fsqbpbsk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zwfajctl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rblqkhqd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlvlqott.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jeclodgn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ixickjdg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zobfzbkh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vevdonub.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3coxjzehd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rxjxvitk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bsgtpvbg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3inzigzfl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ckcnjppu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vvaqhlpl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ngbvwtja.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtjtqj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3uxfkkovh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3loaumbtu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mtzzqdae.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvuwtplm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dtiaincl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kxjxelvi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dpdalwzk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kiezvjkg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vhhjeyex.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hfkemtac.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfiifqa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uctmqsxg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ngtfqhyg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3odcqgron.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rveyoeci.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xgpovtls.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zfuaoqkn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rctedtsd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfuvkiyi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oqjcwqxr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jmojnjmg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kdigosky.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3unsjubpd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cwphlsdt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcwqidy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3quphpmpf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3araesdcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mkpnlhjb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rbpnewaw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3chdhaugn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3boqztpkp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wbtlerft.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yijgoxta.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zwmmlzmu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qluxdrdh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kpfgaukf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktfddblk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ogfstozs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3apreouqw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zhqmkrgt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lmfxzsdh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjltuqyu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lixoblfl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kpyrzbhn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lixfvqrv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qgcqpxmo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytmwkaof.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sgxphnlh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qdmcvsqy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xvhcaefg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hbnaasdi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3noqigivp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uazuhudh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3srtqifdy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3brvherzr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3funrdnjd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qieisavn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fjgbqaij.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xovutdlb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vqnxikvj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgcsrydd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vcnutvgj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3visvbzro.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cquhdhxf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dldopevt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cijemktc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3daqeiqiz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ancrfyre.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibmyatvq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gieendal.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lrryklvt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3waggbqsb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qbqjithq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tnulxwiu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cgjbobkb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kzjzmwga.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3roiwjlqy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiammkm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eudzruhm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lgzjcmtz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lwotsyop.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wdxutikn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wehxonyi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3itnqwvfp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3veqgzlwf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3beahjuec.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3phzmqxvs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gypwitma.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sjdhgftq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3brejbqgf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3htyrstzu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mlshkbfm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pcdbkjub.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3eolyrljc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ioonevfv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vwqjkzvj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qqjjpsiy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mxayabyr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrdmwmjy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ydirqise.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3epvslazn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3okhdhwhw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uhemighp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zatlzvns.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xfjxlwwr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lnbpqfxa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jjxcphpd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ayrbvzev.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rwdaeblr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ielpmqhz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uxothxgl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fvpqpnxx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svopjcrd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqdqnrwt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xwqmxbkt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sarptnvb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ocndatoc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ephedxer.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tjzjjtas.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hmutrvne.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hgmaaoya.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cxswrayn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnhdyjr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fqbebemy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rkundcnb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3akragmqq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3odejhikn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3drjssktf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzthlsev.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3avxrhwfy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfukthsd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3byoxplbd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rlzipxdb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mngmuiby.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nroqrfhk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrcuhki.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jcxklbgj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3citirblz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3awdqiooj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yqhimhhw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fiorvoqh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yctqohma.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpsmtpp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vlpcpgnt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dbwqgjpe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kqxdchph.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pfdlobjr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jlugetzd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wfjrufvq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hkgejoln.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3shnulgjz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pimusgrt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rcbjzqra.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bsxhjuag.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3alubhzhb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ugicnxhs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nwdjyyzv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3usvbxeed.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yjnoeyxw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hkyukake.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3iwhmpmpi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htllykvt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qlejseof.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pandrmag.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bhwyzvyo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gdatdygh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jcrhfsli.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bldlerif.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aushjuzk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nyhlgyxo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtehbxn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zeniwsnr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fqruwviy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gtghhhqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovnrawba.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dudmohxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkkzfkcu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dppoqwch.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3judzjxex.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3josgcsgy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fzbwlqnh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ruewdoni.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxpyivca.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sdvddils.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xgtgeztf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zusdinre.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yyhsxerq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ubjjttbg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yaguauiq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwflywv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrjrtnw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjshrec.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qdowitvg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bpfqtaat.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kevnlqfp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3afohxpmc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lvifudfx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tgccttxg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtvhxksr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fspodoxk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oinlsunl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iqbyxpuz.html


<!-- 参考信息 -->