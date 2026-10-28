代发 wailian999

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtefbdmmrb.html

[R58] 下载文件
来源：http://hz.ivvv.top/gtjshsfiyi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtlfjygjwi.html

[R59] 发 POST JSON
来源：http://hz.zycfv.cn/gtlqoiwdqk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.0kj1m.cn/gtxnvnkbaj.html

[R60] 只看 HTTP 状态码
来源：http://hz.smart0.xyz/gtnlawizew.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guowangkeji.top/gtklrvnlxk.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtlhgozqim.html

df -h;  du -sh *
来源：http://hz.andypj.xyz/gtvufnajey.html

[R62] 找最占空间的文件
来源：http://hz.fzhhl.top/gtiiyiwjco.html

du -ah . | sort -rh | head -10
来源：http://hz.dianchejie.cn/gtdnrbqmrj.html

[R63] 内存与进程
来源：http://hz.yueranfly.top/gtfhxirjhz.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtayhkakbx.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtoodwutfo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daxiang520.top/gtezysoeif.html

[R65] 查看端口占用
来源：http://hz.yangfankeji.com/gtjxotbmta.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gtllrfimou.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gthfbtwyxp.html

crontab -e;  crontab -l
来源：http://hz.wangshuangyany.cn/gtgwpvagkp.html

[R67] 生成随机十六进制串
来源：http://hz.hfpthk.cn/gtidtpsspg.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtvpanviwg.html

[R68] 计算文件校验值
来源：http://hz.yongpay.top/gtxyxcpadb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gaohongyu789.top/gtympcxhiv.html

[R69] 生成随机密码
来源：http://hz.yonumen.top/gtruubezwh.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtimignhtp.html

[R70] 时间戳与互转
来源：http://hz.xziqi.cn/gthzedlirq.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtoqjwcbuz.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtytzbshdg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yonumen.top/gtqjfzlwcz.html

[R72] 等待端口就绪
来源：http://hz.shzxlz.cn/gtfsaohgcj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtlptqivyn.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtufzwvrnm.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtgxshclrg.html

[R74] 批量重命名
来源：http://hz.zhongyouzk.top/gtbvarxekn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dianchejie.cn/gtngifxpkp.html

[R75] 导出环境变量
来源：http://hz.yuxming.cn/gtdabagxdc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tianlin.xyz/gtrbizajvf.html

[R76] 使用临时文件
来源：http://hz.mhx1999.top/gtueivsrdn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtcyzoztro.html

[R77] 读取用户输入
来源：http://hz.xziqi.cn/gtfmefdckq.html

read -rp "请输入: " ans
来源：http://hz.zdqjudy.top/gttuppwntv.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtywktzyom.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtrvusqqtt.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtyeiarykd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aibaodan.cn/gtxhsikpxk.html

[R80] 查看脚本执行耗时
来源：http://hz.ydjk.org.cn/gtkrueswuf.html

time ./run.sh
来源：http://hz.feifeiyinyue.top/gthxcioflb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxtbtlrsp.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtqhfavifd.html

================================================================================
来源：http://hz.316326.xyz/gtcffpwrqc.html

[S01] C：Hello World
来源：http://hz.jinqigufen.top/gtitgpgeer.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtoanmwkyi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtscpkbflu.html

[S02] C：变量与格式化输出
来源：http://hz.iojbl.cn/gtjrrfttjn.html

int a = 10; printf("%d\n", a);
来源：http://hz.cashguo.top/gtqfylzbkv.html

[S03] C：读入整数
来源：http://hz.zhongyouzk.top/gtfaazgfcs.html

int x; scanf("%d", &x);
来源：http://hz.shzxlz.cn/gtytfwuaph.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtpdriftxx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtyvovelhh.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtoilfkhnc.html

strlen(s)
来源：http://hz.cucudq.cn/gtbdmcuicv.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtsieduxbi.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtqzniqkhg.html

[S07] C：数组遍历求和
来源：http://hz.yongpay.top/gtirnzjehd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtcqtpvvcs.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtioekzmtl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gtbgumflqm.html

[S09] C：结构体定义与初始化
来源：http://hz.ydzc1.top/gtpvpbptah.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.kuanghao11.cn/gtijasxhjv.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gtssixxdbe.html

int *p = &a;  *p = 5;
来源：http://hz.aibaodan.cn/gtphycotjg.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gtovladwng.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258888.top/gtefemcztk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhoulong.xyz/gtliddeewc.html

fclose(f);
来源：http://hz.mhx1999.top/gtzjfnjkzz.html

[S12] C：写文件
来源：http://hz.shangyingyoupin.top/gtnvgaejti.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtbwnanqqz.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtqjcmydcr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtycnwtwim.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gtsslyrakx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtuedjtdge.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtymgwlcbl.html

(double) a / b
来源：http://hz.cdnleiting.top/gtmuxtsqwl.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtfrhuicyj.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtubskxbjh.html

[S17] C：安全拼接字符串
来源：http://hz.ydzc1.top/gtloyjqfrj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtibogttrn.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtwtmiujyb.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gttfgiadhf.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtzxsynsez.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtxhjqbkvq.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gtrkmvlfvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtmbbhwjdu.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtwszjbirh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sweek.top/gtdbvucqlk.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gtzoagckdl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtdacxvzfr.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtscbarpev.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtyjkjpess.html

[S24] C：获取本地时间
来源：http://hz.cqqwz.cn/gtdwfkuchk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinyuanbaomall.cn/gtiktuqzoo.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtvebgwvwv.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtdtwogxjy.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtebmhgzio.html

memset(a, 0, sizeof a);
来源：http://hz.zhoulong.xyz/gtcuqzruqy.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtvrhlgash.html

const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtatahzfjj.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtnvvkmusy.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtytygdcbl.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtqjxgibgk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtcvqnynqr.html

[S30] C：头文件保护
来源：http://hz.yj202588.top/gtzeyegqxu.html

#ifndef X_H
来源：http://hz.zhoulong.xyz/gtmjrvzusn.html

#define X_H
来源：http://hz.dianchejie.cn/gtmcqzdtle.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtcuicdnja.html

[S31] C++：Hello World
来源：http://hz.aibaodan.cn/gtmbskjiee.html

#include <iostream>
来源：http://hz.9152youxi.cn/gtiwrmoash.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.0kj1m.cn/gtopjcslzs.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gtutonhvjm.html

std::string s = "hi";  s += "!";
来源：http://hz.hnqzz.top/gtxcnlansp.html

[S33] C++：vector 增删
来源：http://hz.jqgfzy.top/gtmtzhikhw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258.top/gthhzhevyz.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtkntlslwo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtstsnmgjn.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtrhvikowg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtaptzspyt.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtjezpeevb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtixrvemlt.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtakftnkue.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtponuuflx.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gtzymtmqhx.html

std::sort(v.begin(), v.end());
来源：http://hz.jinyuanbaomall.cn/gtbshgetit.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangtech.top/gtquhnptib.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtaswmzwkz.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gtrliafptl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gthfhzntte.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtasjdmzbk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtzdavhyyi.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gtyfjoleri.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtltoyecxj.html

[S43] C++：智能指针
来源：http://hz.nanxuanxn.top/gthglinqpt.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gtepqrunbw.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtbfgyawgt.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtzochmtec.html

[S45] C++：lambda
来源：http://hz.nanxuanxn.top/gtjguwgsqw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cqqwz.cn/gtoutqizuj.html

[S46] C++：函数模板
来源：http://hz.iojbl.cn/gttdbnvglj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cucudq.cn/gtywvrsmpx.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtrvoetolb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.dashuyun.cn/gtdxwonxpz.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtfompfznc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtjgwmrslg.html

while (std::getline(in, line)) { }
来源：http://hz.sufxvd.cn/gtbiniaxqo.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtsbotosdd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hysaishi.cn/gtgfdzcurp.html

[S50] C++：格式化数字
来源：http://hz.chenjidiqi.icu/gtpdgjmrcg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtbjipusil.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtopixgkpm.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gthygtizqr.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtsdewataq.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gthaxuwazd.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtsfzmcqrj.html

std::vector<int> w = std::move(v);
来源：http://hz.c1oappe.top/gtyityiohm.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtyzzbnpuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hysaishi.cn/gtwgrjmzbn.html

[S55] C++：结构化绑定
来源：http://hz.dianchejie.cn/gtmrmowldc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cucudq.cn/gthqbsyigb.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gtfgivyvyj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cheryme.top/gteybkythp.html

[S57] C++：编译期常量
来源：http://hz.cqqwz.cn/gtdixxidoh.html

constexpr int N = 10;
来源：http://hz.jqgufenzy.top/gtjnrdbqoj.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gthchrcwaj.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydjk.org.cn/gtxqfrfahw.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtguktsbnr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hongshengwenyu.top/gtnmscvzvt.html

[S60] C++：遍历并删除元素
来源：http://hz.hfpthk.cn/gtwmonlnvj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hfpthk.cn/gtnmipgqzn.html

================================================================================
来源：http://hz.xylfe.cn/gtnlhlrues.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtjvnjanpo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwaxwlbak.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtxhdbsxcy.html

println("Hello")
来源：http://hz.yj20258.top/gtkibutvui.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtownmjxzh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtjyklnohd.html

[T03] Kotlin：字符串模板
来源：http://hz.guannengcc.top/gtungculkf.html

"值: $b"
来源：http://hz.tian-w.cn/gtctocwxxn.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtvzfmbkfc.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtruqkbetn.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtpqhspezm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangshuangyany.cn/gtdakvmzlc.html

[T06] Kotlin：集合映射
来源：http://hz.cdnleiting.top/gtbdyihgrg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gttiqietcg.html

[T07] Kotlin：集合过滤
来源：http://hz.tianlin.xyz/gtgjkmhzeo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtubzcxzvm.html

[T08] Kotlin：数据类
来源：http://hz.fengsongda.top/gthyansoxa.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtrtwiedqt.html

[T09] Kotlin：扩展函数
来源：http://hz.yj202588.top/gtxjrpvtzk.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtznoxfzjs.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gttlcfszqa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtsjxzgufi.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gttgqvsgfu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jianghu66.top/gtawtwbmam.html

[T12] Kotlin：解构声明
来源：http://hz.zdqjudy.top/gtwckswclj.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtvcuhxabq.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtmgafhvhd.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtbjpqdmch.html

[T14] Kotlin：循环
来源：http://hz.andypj.xyz/gtbkxykhvd.html

for (i in 1..10) println(i)
来源：http://hz.nwbrower.top/gtbdmjwojd.html

[T15] Kotlin：接口
来源：http://hz.iojbl.cn/gtbmcdrynx.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtrgprxncg.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gtqaxhdqce.html

print("Hello")
来源：http://hz.andypj.xyz/gtgkbalizg.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtbnvwhhhs.html

var a = 1;  let b = 2
来源：http://hz.ywan-chungtsiang.top/gtbtxdmavs.html

[T18] Swift：字符串插值
来源：http://hz.cheryme.top/gtyztrotdt.html

"值: \(b)"
来源：http://hz.pycfn.com/gtuasiimpt.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtdntaeqjq.html

if let n = opt { print(n) }
来源：http://hz.kuanghao11.cn/gtxmugebbc.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtbhxsftgv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hysaishi.cn/gtgbagqwny.html

[T21] Swift：遍历
来源：http://hz.hnxiangtu.top/gtkxfejodl.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gttzjiomjq.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtkifdtzez.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gogol.net.cn/gtvrgkbsnc.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gttdqlqchn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ppjwa.cn/gtmizcytjj.html

[T24] Swift：闭包
来源：http://hz.sufxvd.cn/gtwodqcfnf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtbquwqmmg.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gtlacbonfw.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtfakxwlpe.html

[T26] Swift：类与重写
来源：http://hz.mhx1999.top/gtelzmmjsj.html

class A: Base { override func f() {} }
来源：http://hz.ydzc1.top/gtnasnvqdw.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gtoqyoofew.html

do { try f() } catch { print(error) }
来源：http://hz.ivvv.top/gtncdbezgc.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtaibfrcua.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gthnsfxlgo.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtgiyeujbd.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtvscjlwuy.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtgktrruog.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtnvwcoonk.html

[T31] Lua：Hello World
来源：http://hz.ppjwa.cn/gtsuhdlvmg.html

print("Hello")
来源：http://hz.jinqigufen.top/gtfizyztle.html

[T32] Lua：局部变量
来源：http://hz.sxryk.cn/gtaglxtnfa.html

local a = 1
来源：http://hz.ivvv.top/gtrcvdaapz.html

[T33] Lua：表（数组）
来源：http://hz.jqgufenzy.top/gtrzgzxulr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gtjydzrnhp.html

[T34] Lua：遍历表
来源：http://hz.316326.xyz/gttqoukwms.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxinkj.top/gtsoggbuso.html

[T35] Lua：字典表
来源：http://hz.jinghuilouyu.cn/gtahdcomhy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tianlin.xyz/gtjjldspnb.html

[T36] Lua：函数
来源：http://hz.fengsongda.top/gtarglajbe.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangtech.top/gtrqdpmfje.html

[T37] Lua：字符串拼接
来源：http://hz.0kj1m.cn/gtkywcazhm.html

"a" .. "b"
来源：http://hz.shuidangran.top/gtusoveodg.html

[T38] Lua：条件
来源：http://hz.yanxiufei.cn/gtnrlzjrxj.html

if x > 0 then print("正") end
来源：http://hz.yj20258.top/gtatruvgoa.html

[T39] Lua：模式匹配
来源：http://hz.xuetiantiany.cn/gtlbwrcsaq.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtrmvxovhh.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtopovpwcn.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtqpungciz.html

[T41] Perl：Hello World
来源：http://hz.sufxvd.cn/gtzpfclcld.html

print "Hello\n";
来源：http://hz.cheryme.top/gtofiaorvk.html

[T42] Perl：变量类型
来源：http://hz.jqgufenzy.top/gtjnbxhztg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gthlpjsqei.html

[T43] Perl：字符串插值
来源：http://hz.mhx1999.top/gtqrvawttq.html

"值: $a"
来源：http://hz.chenlongwang.top/gtqkehufnh.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtnoynznqu.html

if ($a > 0) { print "正"; }
来源：http://hz.hywenlv.cn/gtsuniswtl.html

[T45] Perl：数组遍历
来源：http://hz.jqgfzy.top/gtzrkqorea.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtsptmvywl.html

[T46] Perl：哈希操作
来源：http://hz.xinyue.icu/gtmjznqjbc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ybcxt.top/gtietiyexb.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangtech.top/gtajaknscy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gtseqtgsbd.html

[T48] Perl：正则替换
来源：http://hz.chenlongwang.top/gtkpsoipzf.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gthpnemxbk.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtkikvdsva.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtyjjtetfu.html

[T50] Perl：逐行读文件
来源：http://hz.iojbl.cn/gtxuipsiez.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hysaishi.cn/gtoxclavkj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cheryme.top/gtxagpbpyd.html

[T51] Scala：Hello World
来源：http://hz.wangshuangyany.cn/gtdzfqwfxt.html

println("Hello")
来源：http://hz.xylfe.cn/gtqlypsgdb.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtqbqylbxm.html

val a = 1;  var b = 2
来源：http://hz.yuanzhike.top/gtvbeizrsi.html

[T53] Scala：字符串插值
来源：http://hz.xylfe.cn/gtcbnscfow.html

s"值: $b"
来源：http://hz.mhx1999.top/gtpksztrrf.html

[T54] Scala：集合映射
来源：http://hz.dianchejie.cn/gtskwnqfvx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangtech.top/gtlhosyuuf.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gtbeiqohcc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xingfuxueyuan.xyz/gtivqnstuq.html

[T56] Scala：样例类
来源：http://hz.wangshuangyany.cn/gtusnbsosq.html

case class User(name: String, age: Int)
来源：http://hz.wangdashe.top/gtzlkogbrl.html

[T57] Scala：模式匹配
来源：http://hz.cucudq.cn/gtnyujbaym.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnqzz.top/gtgaifswoh.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtnxwhwpbm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guannengcc.top/gtvmsizaeb.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtkcvqxpgg.html

for (i <- 1 to 10) println(i)
来源：http://hz.cheryme.top/gtgfnmtdva.html

[T60] Scala：折叠
来源：http://hz.ywan-chungtsiang.top/gtqfjxirpw.html


<!-- 参考信息 -->