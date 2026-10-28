代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtmdeyhqbi.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gtjbqfhwlb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtixpffrrx.html

[R61] 磁盘占用
来源：http://hz.smart0.xyz/gtwiwogicf.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gtptytrawj.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gtvxxrtnes.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gtyyktweva.html

[R63] 内存与进程
来源：http://hz.jlsjyb.cn/gtllxmhunw.html

free -h;  ps aux | grep nginx
来源：http://hz.yuanzhike.top/gtvptehjca.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtqbpfxnso.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtndydpaug.html

[R65] 查看端口占用
来源：http://hz.zhengqikj.top/gteqlvqhug.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.0kj1m.cn/gtqsdsceut.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtbmegqbsc.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtkpowxiee.html

[R67] 生成随机十六进制串
来源：http://hz.nwbrower.top/gtezaiispy.html

openssl rand -hex 16
来源：http://hz.gaohongyu789.top/gtwvrjsige.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtvpdvgdka.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtyxilwork.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtmdnwxtzn.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtmkeerpae.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtmzwivfbh.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gtwmlmyvwf.html

[R71] 日期格式化
来源：http://hz.nanxuanxn.top/gtkmcvegeo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangtech.top/gtefehcuao.html

[R72] 等待端口就绪
来源：http://hz.fengsongda.top/gtqbvkxsdc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtgwsrhwfh.html

[R73] 分割大日志
来源：http://hz.tanke756.top/gtspfugnjl.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtbztjtavi.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtmgnrhqha.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtptoqakxn.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtwwchvmml.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtnqliehqg.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtubfbazug.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtrcrptvmw.html

[R77] 读取用户输入
来源：http://hz.hnqzz.top/gtilclmmvz.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gtmsuazwbg.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gtbmabsmhw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtcgqkulki.html

[R79] 解析命令行选项
来源：http://hz.jinqigufen.top/gtgpgtuajc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtobudhgwz.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gttaxblboz.html

time ./run.sh
来源：http://hz.mhx1999.top/gtlvqahtdk.html

================================================================================
来源：http://hz.yonumen.top/gtttgaksib.html

S. C / C++ 专题
来源：http://hz.jlsjyb.cn/gtrnpyfahc.html

================================================================================
来源：http://hz.guowangkeji.top/gttimvcciq.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtlocvmwar.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtenbiqpwf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yonumen.top/gtsnrstyeg.html

[S02] C：变量与格式化输出
来源：http://hz.hysaishi.cn/gtdxsntiyv.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gtsiipwtpw.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtsogblndc.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtlyuqtdbd.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtgdmrrpyj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gtkxamdqxv.html

[S05] C：字符串长度
来源：http://hz.chenjidiqi.icu/gtqhpsdgrn.html

strlen(s)
来源：http://hz.aibaodan.cn/gtfnxmgqkb.html

[S06] C：字符串比较
来源：http://hz.hywenlv.cn/gtavxcfpqx.html

strcmp(a, b) == 0
来源：http://hz.zdqjudy.top/gtuvhahkhy.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangkeji.top/gtmbfgshsa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtmtdufexz.html

[S08] C：动态内存分配与释放
来源：http://hz.pycfn.com/gtywikjttu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtfhylbolx.html

[S09] C：结构体定义与初始化
来源：http://hz.jiagoushi.top/gtcvqgtegk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gtwsmomirk.html

[S10] C：指针与解引用
来源：http://hz.jqgufenzy.top/gtxzlqjvpe.html

int *p = &a;  *p = 5;
来源：http://hz.cucudq.cn/gtqkblswzf.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtrknjmxya.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gturssorph.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtbkvhhrah.html

fclose(f);
来源：http://hz.hysaishi.cn/gtcsbvswxs.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtfhsktpln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhongyouzk.top/gtdcqajyug.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtbmwfhliz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yangfankeji.com/gtmurgcpyi.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtklmojuyz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtfifkulfa.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtzuvxnuzc.html

(double) a / b
来源：http://hz.gotoacloud.top/gtbirappvs.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtpdynwvmq.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtkpatqpxy.html

[S17] C：安全拼接字符串
来源：http://hz.bjfxy.top/gtyoodubia.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtlvzgijmq.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtmaaqqbfd.html

int main(int argc, char **argv)
来源：http://hz.cheryme.top/gtyppsgeag.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gtojifsuqn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtpxnyomwd.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtcaenqbro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtzmlcvegt.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtkfyzdrls.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gaohongyu789.top/gtnxphmyuq.html

[S22] C：字符串转数字
来源：http://hz.kuanghao11.cn/gtxnhfcsfe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtbdkhqmng.html

[S23] C：随机数
来源：http://hz.tian-w.cn/gtxlgdvjjx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.snrcjt.cn/gtkscmevfm.html

[S24] C：获取本地时间
来源：http://hz.daxiang520.top/gtfpgkltsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtrgfoedrn.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtjaxziwkh.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtizopskxl.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtxvuyuarg.html

memset(a, 0, sizeof a);
来源：http://hz.hywenlv.cn/gtdquwihts.html

[S27] C：定义常量
来源：http://hz.ydjk.org.cn/gtlkivlmgr.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtjcqioqnw.html

[S28] C：静态变量
来源：http://hz.kuanghao11.cn/gtqyqrygsk.html

static int counter = 0;
来源：http://hz.birdmap.top/gtytcbzwpr.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gtpulztyaq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.redwolf501.top/gtuqmqdiat.html

[S30] C：头文件保护
来源：http://hz.gotoacloud.top/gtgvuzfbav.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtjanfyjxa.html

#define X_H
来源：http://hz.chenjidiqi.icu/gtihwqjddn.html

#endif
来源：http://hz.jlsjyb.cn/gtulswesxx.html

[S31] C++：Hello World
来源：http://hz.9152youxi.cn/gtyuxbixow.html

#include <iostream>
来源：http://hz.fzhhl.top/gtixpsjoip.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gthfavxvea.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtmedawaxj.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtvibtqjwl.html

[S33] C++：vector 增删
来源：http://hz.gzhubu.top/gtgxoaximz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtjyjbuwdi.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtebvvkopi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxuanxn.top/gtwukyonrs.html

[S35] C++：map
来源：http://hz.haohaochexian.top/gtrplcwife.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtnfjaurte.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtwwdnadlm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtxvaeqtfb.html

[S37] C++：set
来源：http://hz.tanke756.top/gtdufypmqr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtmohggicw.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtrtxbssjx.html

std::sort(v.begin(), v.end());
来源：http://hz.jlsjyb.cn/gtoyqcynot.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtavswbinh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtsgepunwm.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtkuzdwozo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtzojurlyw.html

[S41] C++：类与构造函数
来源：http://hz.cqqwz.cn/gtgiftdzdp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtqxqfjfdx.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtnaxfojmx.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtiahzhdcd.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtmjadzrni.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtbfakkqhv.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtimqoyyil.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtrvskfrgc.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtzqppirbz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtzkdjrlyf.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtihtzbrzi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sysykeji.top/gtoqjgpqrp.html

[S47] C++：结构化绑定遍历
来源：http://hz.redwolf501.top/gttzbmbuxe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtuphewctg.html

[S48] C++：逐行读文件
来源：http://hz.aibaodan.cn/gtboyswtmn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtqhqcykux.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtiamqquxs.html

[S49] C++：写文件
来源：http://hz.xinyue.icu/gtejnxbkhb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pycfn.com/gtkisehpzp.html

[S50] C++：格式化数字
来源：http://hz.chenlongwang.top/gtbxvpqffm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtfzwfegnn.html

[S51] C++：显式类型转换
来源：http://hz.bjfxy.top/gteaozbhqj.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gtyltyapsd.html

[S52] C++：const 与 noexcept
来源：http://hz.dianchejie.cn/gtoiwypyxv.html

int size() const noexcept { return n_; }
来源：http://hz.redwolf501.top/gttgbxeyfz.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtleptpwpv.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtejetnlva.html

[S54] C++：异常处理
来源：http://hz.zhoulong.xyz/gtzmhjjoap.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhongyouzk.top/gthjrknvdw.html

[S55] C++：结构化绑定
来源：http://hz.meibo888.top/gtetpivwbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtkqcxekpi.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtlohgjupf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenjidiqi.icu/gtdvysrfxj.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtvccymesb.html

constexpr int N = 10;
来源：http://hz.jinyuanbaomall.cn/gtymttvjhx.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gttssnistb.html

namespace ns { int f() { return 1; } }
来源：http://hz.jianghu66.top/gtrrcowujd.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtiryetmpw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtcsrdrmbh.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtcmmbojdc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yangfankeji.com/gtpacubish.html

================================================================================
来源：http://hz.yuxming.cn/gtrvsokjbt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtnkybuawb.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlxleatsz.html

[T01] Kotlin：Hello World
来源：http://hz.cucudq.cn/gtguqynhto.html

println("Hello")
来源：http://hz.fzhhl.top/gtzzqnpsmg.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtaaxkmjfx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtgpbkjzbg.html

[T03] Kotlin：字符串模板
来源：http://hz.jinqigufen.top/gttiiynmso.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtatxcqdcq.html

[T04] Kotlin：空安全
来源：http://hz.yonumen.top/gtoqdjtnwd.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtmnricolf.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtwwrghhev.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtmkymfhrd.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtfklfkyqf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cdnleiting.top/gtemxzpcxi.html

[T07] Kotlin：集合过滤
来源：http://hz.fzhhl.top/gtshxwrjjn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gthtymzppt.html

[T08] Kotlin：数据类
来源：http://hz.yueranfly.top/gtwkfdivdb.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtjfctkgge.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtjctyxsrl.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtxzxtdqbg.html

[T10] Kotlin：默认参数
来源：http://hz.hysaishi.cn/gtbcmqphhr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtoddgdixu.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtxxyzhczv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtisowmddi.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtlvvpirmk.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtnigvvhoh.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtpqnulbec.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtfyybwbos.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtisxjolzq.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gtfldnuixn.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtuerphnhq.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtljvcykob.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gtojqcgcta.html

print("Hello")
来源：http://hz.gogol.net.cn/gtyyloanpv.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtylbdkzhu.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gtwlpcgwxn.html

[T18] Swift：字符串插值
来源：http://hz.hnqzz.top/gtyxinkezm.html

"值: \(b)"
来源：http://hz.gaohongyu789.top/gthxwmifnq.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gthgangmri.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtlubpyfcg.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gtrfmybchr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yongpay.top/gtvwccyexe.html

[T21] Swift：遍历
来源：http://hz.jyoumei.cn/gtnxrpnwjy.html

for x in a { print(x) }
来源：http://hz.shzxlz.cn/gtsccmdhur.html

[T22] Swift：字典
来源：http://hz.xuetiantiany.cn/gtupzzztup.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gtvguxvrmt.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtsoowavcg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jiagoushi.top/gtbatwgcwc.html

[T24] Swift：闭包
来源：http://hz.wangshuangyany.cn/gtcopfpoia.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dashuyun.cn/gtoxbfyazm.html

[T25] Swift：结构体
来源：http://hz.jianghu66.top/gtebxpcrmn.html

struct P { var x: Int }
来源：http://hz.ywan-chungtsiang.top/gtywcqnrgn.html

[T26] Swift：类与重写
来源：http://hz.jinqigufen.top/gtejasufjx.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtrunopawy.html

[T27] Swift：错误处理
来源：http://hz.xuanzx.com/gtprazpyan.html

do { try f() } catch { print(error) }
来源：http://hz.nanxinkj.top/gtwhirtocf.html

[T28] Swift：枚举
来源：http://hz.zhiwuduotai.top/gtbkpgyxhr.html

enum Color { case red, green }
来源：http://hz.snrcjt.cn/gtpnhtrkaw.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtwjfjagxx.html

guard let x = opt else { return }
来源：http://hz.zycfv.cn/gtmllevrmh.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtxkybumym.html

protocol Shape { func area() -> Double }
来源：http://hz.jinyuanbaomall.cn/gtczrglslb.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gtfypqvspn.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtywaqlwfs.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gtinbtkaja.html

local a = 1
来源：http://hz.ywan-chungtsiang.top/gtpnpsuwve.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gtywzgkfyh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.bjfxy.top/gtoldazckp.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtnpsbunvs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gteqdnsota.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtziqnfeai.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuetiantiany.cn/gtesoebhkd.html

[T36] Lua：函数
来源：http://hz.xziqi.cn/gtpieatxuw.html

function add(a, b) return a + b end
来源：http://hz.xziqi.cn/gtodcmzxca.html

[T37] Lua：字符串拼接
来源：http://hz.hammf.cn/gtzehuwoik.html

"a" .. "b"
来源：http://hz.ehwqpu.com/gtmodijipj.html

[T38] Lua：条件
来源：http://hz.nanxuanxn.top/gtyybrbwld.html

if x > 0 then print("正") end
来源：http://hz.redwolf501.top/gtduusasxf.html

[T39] Lua：模式匹配
来源：http://hz.sweek.top/gtogboejdt.html

string.find(s, "%d+")
来源：http://hz.andypj.xyz/gthzfncdsl.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gtbxsuowdj.html

setmetatable({}, { __index = base })
来源：http://hz.zycfv.cn/gteaclkabq.html

[T41] Perl：Hello World
来源：http://hz.yangfankeji.com/gtzonrsaxo.html

print "Hello\n";
来源：http://hz.cheryme.top/gthblumwpp.html

[T42] Perl：变量类型
来源：http://hz.0kj1m.cn/gtagpyqmdz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangshuangyany.cn/gtgzobjqaw.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtbffqxuxw.html

"值: $a"
来源：http://hz.0kj1m.cn/gthjwlzmuw.html

[T44] Perl：条件
来源：http://hz.zhiwuduotai.top/gtvhmxfrmb.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtxkieotwu.html

[T45] Perl：数组遍历
来源：http://hz.gogol.net.cn/gtdqdzsjsa.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtolyzeynn.html

[T46] Perl：哈希操作
来源：http://hz.tanke756.top/gtjmemhtvi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xingfuxueyuan.xyz/gtyftaojwh.html

[T47] Perl：正则捕获
来源：http://hz.havefunace.top/gtpoxoebxv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gtheyussnq.html

[T48] Perl：正则替换
来源：http://hz.zhoulong.xyz/gtlrmvwbml.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gtivicuyss.html

[T49] Perl：函数
来源：http://hz.ydzc1.top/gtdeylfgpy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jyoumei.cn/gtsfhbaasv.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gtfjedfrxe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinghuilouyu.cn/gtogalasyg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.vqdsnc.cn/gtbpjlhakc.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtrhijidnr.html

println("Hello")
来源：http://hz.ybcxt.top/gtprzhbbif.html

[T52] Scala：变量
来源：http://hz.chenjidiqi.icu/gtsymsewrx.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtslxhqxit.html

[T53] Scala：字符串插值
来源：http://hz.jqgfzy.top/gtpyrvfptd.html

s"值: $b"
来源：http://hz.c1oappe.top/gtjxpuvyoq.html

[T54] Scala：集合映射
来源：http://hz.vqdsnc.cn/gteeemltcw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gtgukclapt.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtrodorphn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hnxiangtu.top/gtaffuimfs.html

[T56] Scala：样例类
来源：http://hz.chenzaomai.com/gtfdhofhrw.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtiqbjdlzf.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtnwvklfzw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jiagoushi.top/gtrxfltmuz.html

[T58] Scala：函数定义
来源：http://hz.zhoulong.xyz/gtlcholcfz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yvedp.cn/gtckokdtiy.html

[T59] Scala：循环
来源：http://hz.hfpthk.cn/gthevctoty.html

for (i <- 1 to 10) println(i)
来源：http://hz.feifeiyinyue.top/gtjopiomrw.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtzcjxesjn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.pycfn.com/gtjllwnjxy.html

================================================================================
来源：http://hz.aizwys.cn/gtbfbsefdg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtvknkjgna.html

================================================================================
来源：http://hz.yangfankeji.com/gtwgznqbhc.html


<!-- 参考信息 -->