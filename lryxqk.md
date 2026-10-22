代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2daitncst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cryvxjpo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2inmrjdpz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhuijojo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adxjnmlx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2idpoektn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2draoykwc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mfjejwqm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2koefdzpf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2csivzulm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ridrehkz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iqeikhxr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ylenhrdn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xrtjnvyr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jvaajprb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hhemdjrs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2iubicaar.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2roxhwpnf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ebqdtydx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hondhjxo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wlxkxkgt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwifekhg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uqzhxuxw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rnmlzdyd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bfimrwoq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ybqhpvtr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tqinzyde.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wwfpgfux.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nluryezl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pplwdxiz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gzkggggb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ltqzgwyz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gbyzyntx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cozdqixo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nuwygvqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwflpllg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2utepfxik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcqhcptv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iygeilyz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zuwhkfuy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2eqaidlji.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2myfyphdk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xpybgbnw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wnhdumnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fxoebhjy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gquzhrsw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lvcwluwd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dondonqh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fsfattcj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nwnzycip.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bezwbycu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qauqdzyc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fhacruce.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kytlpdxl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2taflpzql.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nvhljwsr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dpsxqjya.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zpnozhbr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sxrrsqug.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kwyngtgb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tcduwfus.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2klrduapc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fudhekaa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2artjbryd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gyujsuas.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aidqkrun.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqsyouxo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxefpzmq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uoxzadqi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lmczjwhr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2akrqncvw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2thcxcovs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kpbeesbv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnjwuqcw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wodmkptl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mkybajsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hmrodloe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fgckvdue.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mmmbcpqk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ocjuvwck.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aaqyammu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2waohbrnk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ahrciqdv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xbvqybnz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vwwaunhb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vdadcnpf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xpsgivzi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bgqefgwn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vjtjxfwc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcnypqj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ifopibnb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ujvtaher.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2shflyfpe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2emlzqldd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gezafikr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2krtgjgqg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ooyiazvu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jbrxpvsq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cjecmxej.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gihqfmfn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uuqptrjz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vbbaekic.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eafegnbc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2odybzsnq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lpinwigf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rlkhjsji.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2paqxtork.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbfezyp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hmwzdmfr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ohcsrnix.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bqxwwqmf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dqfudjnz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hkpundjt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vzlprkmd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qksypvxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2smfyrkni.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svcmmqsm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yzijbity.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sidyhfzm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lsvtzawn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2edmzfwjg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nsqzvkwc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fputooot.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bagnkybf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2krjkvoyb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ypdnndcu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qngaioze.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2naiqdwcd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hqiqoidm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2syivvuuy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvasynke.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2geuxbmxe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2reynzrly.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpchajo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tbdeldln.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pknyyzkg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2spclszkc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lhifmrbg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nwdkzwlk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bagdetgm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjkidig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hdrsmyji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cphfrwff.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2akwlikxi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbymyhha.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2axqhuhsq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xxyifzzz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xouovnky.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2izoivfda.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgsmnwf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2salildur.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmtkdtqp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qzdaplsz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2aklmpxes.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwnkgpwb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jbwkndxl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jixqjwwd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lvrrnrqd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lylkuhnd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2esyfowsk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zezbbazn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sucgxlrd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhuizen.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2djoqjbul.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bcigdwas.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wsmkjakq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nqkdcdki.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dfkxtvon.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rcwcxslk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xbytyuai.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jfdjrdpu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ikeraurt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hrqqooyt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uoulwffn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmwrhib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mnjadcjs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oxhtklul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fawokrcd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vgufwtka.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eeldmlbx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cbhnwold.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kzkgpqxu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ubjnmczh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2smbcxcaw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2quxgfaay.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfkhkcc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2udsbmwwk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tkquoyed.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjunpjy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wgzagsjc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pykjchha.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kznylvnt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mvrkodlp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xggwiwvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fsnjejrj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2odockytz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qglhodnu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2huldmfyp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2htlekyux.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2osgwawfw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mddmcskr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2flqvycqk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hzizsrvy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2iiudryaq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xarpsaoz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2egliotzs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wjbiuial.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2medwlirx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bcqeiayo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vowdbkla.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fopfuhqb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wclabzej.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uwdflxwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xkjyghcg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vgmrqlje.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lxjtclkt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cuxcptye.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mwmagaty.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2czfzgrqe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rssgtkdm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pororhwg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pwktueru.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cudbctbc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xoidewvs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcadppjn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2davntmet.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqmgqitj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bexahdnu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drsyjyui.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2knteqwnh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejavszwj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uggnainq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fsgnektu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lfxsbfca.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pmefejxc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qmzozbaj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qlgmwlfg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nhdaaxzq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ajuhzqor.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ldtfajfq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cmilurzq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vcspmilv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ruwprxua.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bvogargl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2grymjldk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rqkzcrfd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hjypnxhy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ixisuydh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpdjvsw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vweyywuy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zbvjzvnb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cshuvkaw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2imyvjdcd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jcrnoywv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kgqapvnw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kemqnbgb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wvwgyrhj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsljblg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ikstvrpg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yhjzacst.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vgtjqktu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxsbzirq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cctdyskc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drefzrne.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pedbxsrd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2klvfmshf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2icldgwjv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nbbxwlms.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tcdemspp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mwdezfel.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bydcfome.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2riouhjci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlydrpex.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jhdxiubv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xaasbvnf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmhdqtlp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wfrxqiiw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wivozyma.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xdwqxwqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qfwqpclk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2rjtcgeco.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bcjnqkei.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hfvozujw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2npclbtqx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gvnomylq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2spuwuyki.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2irrzwfrt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cteocpsq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjixggvt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sjusghpd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzxdzfi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wpgdhgpy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zrcqtefs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jgaalmst.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ngttjfyd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ercrlxls.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2goctlbzq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdhfdys.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2povaxodd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wuhalpkk.html


<!-- 参考信息 -->