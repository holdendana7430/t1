代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ywducjew.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2apzckjxj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2egsqebld.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lgqecotl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pwnesimz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tfpftees.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ucpcnlxm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2qxekucek.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cphndpeu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ajcmdllq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kckmsqjj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2euydmian.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2acaqnyaw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ikehwtuq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eyjfoxgz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdarghb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcwmfyan.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jxkoutmr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fikdgvwz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sjvrsznn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gezojebb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gllscysz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tsgaxzpb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zrgekyjs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzxnuyvi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwyhnoup.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbeseex.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ljwfgbpc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gibfcswc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmqvjnxj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tvltotlf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wejecpsx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlrlnaat.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2abptsqpd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iohijrsx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aqzvovai.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zljcwtqb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jftsqieh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ictvajdi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mnjqktmn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tdgxjooy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sphongyh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dtyuhceo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbljhblc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hnweqmtm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhxqywsh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owzkrkds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gggiggez.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2glmydqam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhfpskwk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vhgnbjpz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jzdbqekd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xtnzhjgk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ohlcbmyx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qynuykjs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dbqhgvdj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pkjavmwg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jqpprlpe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2btybefna.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hptmvlvj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ttbwntcb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqmvdziz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fxnmdxbf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rsngalsc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qjxhynhy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cbjwiyym.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jesejmft.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kqoyrjpe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2smigkrkq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dsdfvprv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xexfqivu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bxsrfuxq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kmrzzqyr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aomoanol.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2aqywrmos.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgqlvrt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ianvfynp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmloiz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pbxlwgsw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npzkiahb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kihrtgxo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jrpibjki.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhezhfa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nqbwlmui.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xyrekulz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xbzkdwet.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2oyafahvw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jqcxnlmx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zsiuxhab.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xfvkuroy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2snrqhhii.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hrhdzjjy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rsoyzjin.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lvsapyux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wdilthsu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2psoewoml.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2csoirycy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2suaxvmtm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qznvsfdz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ltmglqct.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gmyotveo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijopqwdr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wuuavisk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2eydqhfka.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zxcxfzfd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2onraitil.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yruymdiw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iqlmrdwl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nahzvihg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uydehlkz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jvtowulk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sghmrrib.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vwqwrdfd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kocikluu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nrwsouct.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fleuzbvl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qhzkirsq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vzkxjzqo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uxluqbul.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ylhwxzva.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ejiknvex.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yificxqc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kaayqwri.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bcywgaci.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ccfjlsrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2utntizgr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lmjjenrl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dhgcyfxm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcarhxxi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uhakhezm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2biyspcyn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pcsncrom.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2owwboubd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bffqsrjw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bdmucwoa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2meqbaubi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cmmpdqcz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2eysgdbuu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kvweaggq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nkvsbeqx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cowgxwve.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rhsfmbwm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtdqsilz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rrygcfqc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fgupbrvu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ksoeqtur.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wucrwfvj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2umkbuzlk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qltzonuz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wnviazba.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2scsnjyaw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxyyldws.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfckiauk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vcnfgsee.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nsjrdgvv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxprhgx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjcmhlw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2kttrkcdp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qiycjjoh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2efhzsrqs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2idbcwtzt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dvquarsd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrxtnqru.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkbkyznt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fclxqipl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqzykfa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zsysfbue.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2sgfhmwhi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bitobrwl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ctlerpcb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsryrks.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pitlpowp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zxiogfol.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2chywvfcd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbcjymfj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oqtrpdqq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dalgbroc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aaaartgy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcvhhdfy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kegrlsyw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fzopbrsb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ansprhrq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2meajhbms.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lvrxyczc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnhwph.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2crrhviwy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kepzpkjw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xjfmaphz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxriupo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwtedvl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sdzitdnb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dhqpumep.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ghedgoeq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ixzdvmsh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wuyjshyt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycwwhndm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gwlmsumk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lyklpuhc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sknpyrbg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zhvbdltc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kunxbwae.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nycuggyx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2auiftzah.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tiaagftz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cvixoktw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2scdnyrbr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nbwwooer.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gfqpsuuc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rewzaxed.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iaxogwwb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ozjswcnv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqhyjedu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yjxjexin.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qtwqzfbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2urghuhab.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ovnvykri.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kkabukpf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2fwnbrtam.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nqtiiidk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zlpbkstl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nlvljlpd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2udunexip.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zggcyyvl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iejmwsun.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zoqlpirc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hrszaabz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dmzxzepo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sdcjhldy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fdvpcwsv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fqnzfvne.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tnpmigzw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2veackopz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qaobnlmz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lidaxpjt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kemargyu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbylmgg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zhllzhec.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qniywqvp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lncgcmxk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2veacxaat.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmvqzkhq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lqffbswn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxvvulud.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rurbxbpj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wpwspkfh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2apvdgumd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2raxnvkzs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zagznand.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2puireopj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2givrfupt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hmwazuln.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdtmqpi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdofniv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kytirxum.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vkbdytdz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gwrcwzcz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzfkujs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2oapcxmca.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwxziqx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxnikty.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nimccyob.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wiulqlel.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lylazmzz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2akusyfji.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iemisfjy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2yfysovvj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hshjulto.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oqhdjxnd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2urqqgqin.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2chabpcoy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ducyfajv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rrvpogof.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ckaqbxcj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fmqgerfb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mnfkkebb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjukgfzt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ybgsoewt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hjqaujhi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tsaxnrmm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ggllzkhn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gdikwqae.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eqnmtadu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fcjfyzbf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2blaiudtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqhzvtyg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2akzlplhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqjvbnhk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gmuxjujr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gordxcal.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xmrbnott.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2njpwkcra.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nkqpgwjy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2euonxfcy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2llugulpw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wswzkodb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulxytqql.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cpxlpted.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gzbjdmdr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nkspbnin.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ejiiwlzr.html


<!-- 参考信息 -->