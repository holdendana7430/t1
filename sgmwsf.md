代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtzppfsamk.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtfglvurrj.html

diff a.txt b.txt
来源：http://hz.yuxming.cn/gtfnsbksrb.html

[R55] 压缩与解压
来源：http://hz.wangshuangyany.cn/gtgiqpnvsi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenzaomai.com/gtiuxzjgcc.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtuhocvlxw.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gtqezymwyc.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtafhtievt.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gtkmabpexi.html

[R58] 下载文件
来源：http://hz.sufxvd.cn/gtyxvdessl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guannengcc.top/gtxngaelka.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtfsfqgczw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtfufksurl.html

[R60] 只看 HTTP 状态码
来源：http://hz.316326.xyz/gteomttmxj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtmakabtma.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtzjkqtgwx.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gthmagxiwi.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtnpiyynix.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtflgriime.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtkribsvnx.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtfhjmaxyg.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtawonlfkr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xylfe.cn/gtkmdbgabq.html

[R65] 查看端口占用
来源：http://hz.nwbrower.top/gtwornadrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtwfbjlsrg.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gtzcnanmze.html

crontab -e;  crontab -l
来源：http://hz.zhongyouzk.top/gtkycrvxnc.html

[R67] 生成随机十六进制串
来源：http://hz.aizwys.cn/gtwjlkgckh.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtndnhxkfg.html

[R68] 计算文件校验值
来源：http://hz.hfpthk.cn/gtroemydkp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydjk.org.cn/gtsqnlxlrx.html

[R69] 生成随机密码
来源：http://hz.fengsongda.top/gtluchofbf.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydjk.org.cn/gtthxbvbxk.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtnkeiucco.html

date +%s;  date -d @1700000000
来源：http://hz.hammf.cn/gtakxczaqf.html

[R71] 日期格式化
来源：http://hz.shuidangran.top/gtlhjofikn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gtbkkqvthk.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtlohdwvjh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daria6918.cn/gtuprxyxnk.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtbmqgsqyu.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtrsdgqerv.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtgyumafkm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtcvfnvcof.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtvbrvlfin.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jyoumei.cn/gtgwvzbhgu.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gttdblfijz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtrlcutenp.html

[R77] 读取用户输入
来源：http://hz.xingfuxueyuan.xyz/gtjhyxymij.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtzgmqhcul.html

[R78] 交互式菜单
来源：http://hz.mhx1999.top/gtvfcmquui.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sxryk.cn/gtikfvlmqj.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gtijdmlddz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gthzgxodru.html

[R80] 查看脚本执行耗时
来源：http://hz.cucudq.cn/gtppkbgzxe.html

time ./run.sh
来源：http://hz.fzhhl.top/gtnehisuof.html

================================================================================
来源：http://hz.xinyue.icu/gtkxbnuakc.html

S. C / C++ 专题
来源：http://hz.xuanzx.com/gtcfcjiixt.html

================================================================================
来源：http://hz.dianchejie.cn/gtyzgnxxdb.html

[S01] C：Hello World
来源：http://hz.cqqwz.cn/gtimkhqjyy.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtorzzqgur.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtlqbvvdgt.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtgpfgiups.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtemhuesuo.html

[S03] C：读入整数
来源：http://hz.chenlongwang.top/gtqpbvlojq.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gtlxxovdgw.html

[S04] C：字符串复制
来源：http://hz.aibaodan.cn/gtlyzcuaiy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ybcxt.top/gtnlbntbps.html

[S05] C：字符串长度
来源：http://hz.andypj.xyz/gteucvubog.html

strlen(s)
来源：http://hz.guannengcc.top/gtbywiypbg.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gtwkqqjjpv.html

strcmp(a, b) == 0
来源：http://hz.aizwys.cn/gtjmzavwsw.html

[S07] C：数组遍历求和
来源：http://hz.yj20258888.top/gtqjwkomdy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtuzhwfwrw.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangtech.top/gtnddlhtcy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtlnmgntui.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gtmwmkbmkm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxinkj.top/gtfeqflgvk.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangkeji.top/gtfvuqilbe.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtuhdrkjax.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtsfbkwlue.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtzrxcilgz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtviveilzt.html

fclose(f);
来源：http://hz.yonumen.top/gtdjakenvu.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtasftvqvt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtyjmlqayh.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gticssywvx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtoflnalir.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtptnaigvm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gttksgmdue.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtswlnkbdb.html

(double) a / b
来源：http://hz.snrcjt.cn/gtsivgtohl.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtoryczwke.html

x |= (1 << 3);
来源：http://hz.fzhhl.top/gtimxrqlkv.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtdwydakcb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtalcrvdzb.html

[S18] C：命令行参数
来源：http://hz.yj20258.top/gtfcataksi.html

int main(int argc, char **argv)
来源：http://hz.vqdsnc.cn/gtqwyzpchi.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtarsqlzfg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtocfpirzk.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gtqwzfktss.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtuunyytld.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtbecqlecd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yongpay.top/gtunutjlmi.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtnwyjqqog.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtjxplpgfq.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtyzgftfti.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtovzmvdlo.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtvsxpibql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.redwolf501.top/gtltcitbub.html

[S25] C：内存拷贝
来源：http://hz.jinqigfzy.top/gtigqqnwkt.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtcuomkvdy.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gtdjaphyyy.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtsgdgfmwc.html

[S27] C：定义常量
来源：http://hz.sufxvd.cn/gtqfjxmwfq.html

const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtlorbywyh.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtpgcszgam.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gtwpornhdg.html

[S29] C：变参函数
来源：http://hz.yuxming.cn/gtyahihtsq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtefvylvvj.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtdmyffkmk.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtnwdddkrb.html

#define X_H
来源：http://hz.yj20258888.top/gtwfyekqwf.html

#endif
来源：http://hz.jinqigfzy.top/gtyecnyywh.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtbanefpmy.html

#include <iostream>
来源：http://hz.xziqi.cn/gtsdrnjwsj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gzhubu.top/gtxsbjmymm.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtrkfeqhpv.html

std::string s = "hi";  s += "!";
来源：http://hz.wangshuangyany.cn/gtuhbdqoeq.html

[S33] C++：vector 增删
来源：http://hz.chenjidiqi.icu/gtwbxtjpzd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daxiang520.top/gtqmpjmpff.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtnuagfyyb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hywenlv.cn/gtnqlabibw.html

[S35] C++：map
来源：http://hz.sysykeji.top/gtelrvjlpm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtbqzymjnw.html

[S36] C++：unordered_map
来源：http://hz.ydjk.org.cn/gttdvfjlva.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtkvekrqtu.html

[S37] C++：set
来源：http://hz.vqdsnc.cn/gtgwmfkeqs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.kuanghao11.cn/gtspclpgvi.html

[S38] C++：排序
来源：http://hz.shuidangran.top/gtgixkmdpf.html

std::sort(v.begin(), v.end());
来源：http://hz.tanke756.top/gtlemarcic.html

[S39] C++：自定义比较器排序
来源：http://hz.guowangkeji.top/gtkmajdluv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tanke756.top/gtblqwcywc.html

[S40] C++：查找元素
来源：http://hz.sweek.top/gtnrteqlln.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtbmbxuwla.html

[S41] C++：类与构造函数
来源：http://hz.kuanghao11.cn/gtydcheylr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtwxcgnjei.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtfzybmvjd.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtyetgjgdg.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtcztsmnqn.html

auto p = std::make_unique<int>(5);
来源：http://hz.ywan-chungtsiang.top/gtpcvmwdct.html

[S44] C++：引用传参
来源：http://hz.xylfe.cn/gtezhvznbn.html

void inc(int &x) { ++x; }
来源：http://hz.vqdsnc.cn/gtpiixefbh.html

[S45] C++：lambda
来源：http://hz.jinghuilouyu.cn/gtdyuzxatg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gaohongyu789.top/gtxojifoyi.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtcyqnkdji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hysaishi.cn/gtashqdxne.html

[S47] C++：结构化绑定遍历
来源：http://hz.jianghu66.top/gttpefojzz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.feifeiyinyue.top/gtkprgmjnl.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gturimwvut.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtiwbttefs.html

while (std::getline(in, line)) { }
来源：http://hz.shzxlz.cn/gtgimivlsw.html

[S49] C++：写文件
来源：http://hz.quarkkingdee.top/gtctblymys.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtkdopkdth.html

[S50] C++：格式化数字
来源：http://hz.chenlongwang.top/gtbmyhtvmg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gterglzzqf.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtcmrinren.html

static_cast<double>(a) / b
来源：http://hz.gzhubu.top/gtfskedwix.html

[S52] C++：const 与 noexcept
来源：http://hz.wangdashe.top/gtncvyhuka.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtdnwxumws.html

[S53] C++：移动语义
来源：http://hz.xinyue.icu/gtqfydupde.html

std::vector<int> w = std::move(v);
来源：http://hz.zhixingplan.top/gtxpmqorkm.html

[S54] C++：异常处理
来源：http://hz.chenjidiqi.icu/gtlgwfqpzj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zdqjudy.top/gtvjirnqxw.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtblyhlfzj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hongshengwenyu.top/gtxrntjbal.html

[S56] C++：optional
来源：http://hz.ydjk.org.cn/gtojevciwq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.kuanghao11.cn/gtcqnigjjt.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtfddpbzpy.html

constexpr int N = 10;
来源：http://hz.svipenyu.cn/gtemtafyqg.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gtoszcdgkn.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtziauhihn.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtmjovxpwg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtcmbbvbtf.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtmwpntfno.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtpebegkrs.html

================================================================================
来源：http://hz.c1oappe.top/gttvvswevn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xinyue.icu/gtxdvqrgdh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdjuhijwz.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtyqyptahb.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtygkxjarv.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtlsfaoqun.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gttunazxdv.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgfzy.top/gthykilonu.html

"值: $b"
来源：http://hz.yuxming.cn/gtmrmvtsro.html

[T04] Kotlin：空安全
来源：http://hz.jqgufenzy.top/gtvcylmjaw.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtzxccgtzh.html

[T05] Kotlin：when 表达式
来源：http://hz.fzhhl.top/gtdaxpdwua.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sxryk.cn/gtdszfzxdr.html

[T06] Kotlin：集合映射
来源：http://hz.shuidangran.top/gtirbjqzjd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ppjwa.cn/gtcmkidaps.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtwpfwgonf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gtylfninir.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtmloamhsj.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtshvdauco.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtubfwjlpq.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtxzlgmolg.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtpxqukxpm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtrmayocqi.html

[T11] Kotlin：协程
来源：http://hz.gaohongyu789.top/gtrylmbktv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gtfiwqavrh.html

[T12] Kotlin：解构声明
来源：http://hz.tanke756.top/gtsrbmyqgo.html

val (a, b) = Pair(1, 2)
来源：http://hz.ivvv.top/gtwbqwyphg.html

[T13] Kotlin：只读 Map
来源：http://hz.wangdashe.top/gtwfpywsig.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtebbfdlqc.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtfrpqglye.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtvcbflomr.html

[T15] Kotlin：接口
来源：http://hz.jqgfzy.top/gtrrfyylce.html

interface Shape { fun area(): Double }
来源：http://hz.zhaomingkeji.xyz/gtcjgdvhyu.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtwghntwzc.html

print("Hello")
来源：http://hz.jinqigufen.top/gtldsaslyb.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gtyhweonfe.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtlzhvbxxt.html

[T18] Swift：字符串插值
来源：http://hz.jinghuilouyu.cn/gtllpupcep.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtawawbmgc.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtvswedngr.html

if let n = opt { print(n) }
来源：http://hz.cucudq.cn/gtbbjdagri.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtybbzhgxj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gthvlgqzni.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtmggnnxuy.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtvsythaft.html

[T22] Swift：字典
来源：http://hz.snrcjt.cn/gtoncslbak.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gotoacloud.top/gtdfclzrui.html

[T23] Swift：函数
来源：http://hz.pengpengdd.cyou/gtcsvekabo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.iojbl.cn/gtnbbbkvtd.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gtultjhwud.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cashguo.top/gtbnhioify.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtkjhmpqev.html

struct P { var x: Int }
来源：http://hz.shanyushiyangkeji.top/gtijjubqkc.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtgfytqswx.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtadwykyoj.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangtech.top/gtbwvzrgnj.html

do { try f() } catch { print(error) }
来源：http://hz.ybcxt.top/gtowqxlvfg.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtfhuraqed.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtfchbkimw.html

[T29] Swift：guard 提前返回
来源：http://hz.xingfuxueyuan.xyz/gtgwuvcaeb.html

guard let x = opt else { return }
来源：http://hz.jiagoushi.top/gtpdvemmtd.html

[T30] Swift：协议
来源：http://hz.xuetiantiany.cn/gtrgcargla.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangtech.top/gtklygsoat.html

[T31] Lua：Hello World
来源：http://hz.yuxming.cn/gtrutkkpgs.html

print("Hello")
来源：http://hz.ydzc1.top/gtcdqoljst.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtqsqzdciu.html

local a = 1
来源：http://hz.yanxiufei.cn/gtxnivdpfn.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtcqoohczf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtplobbvab.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gteziajzpy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gotoacloud.top/gtahpeoixn.html

[T35] Lua：字典表
来源：http://hz.fzhhl.top/gtezsmziye.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtzonfgysa.html

[T36] Lua：函数
来源：http://hz.ehwqpu.com/gtomhhfnhj.html

function add(a, b) return a + b end
来源：http://hz.ybcxt.top/gtcmgoodgy.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gttkgdbdxp.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtcblagyeu.html

[T38] Lua：条件
来源：http://hz.xziqi.cn/gtxgkzhyjs.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtnoihblne.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtjffebmoe.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtbsxxgywy.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtdiodmfqw.html

setmetatable({}, { __index = base })
来源：http://hz.ywan-chungtsiang.top/gtutklviuh.html

[T41] Perl：Hello World
来源：http://hz.cqqwz.cn/gtzslpgfuv.html

print "Hello\n";
来源：http://hz.xinyue.icu/gtoqwmoijh.html

[T42] Perl：变量类型
来源：http://hz.dianchejie.cn/gtxnjrrfii.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.smart0.xyz/gtqeblqwhg.html

[T43] Perl：字符串插值
来源：http://hz.snrcjt.cn/gtfxjpgwpq.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtopbjyqyq.html

[T44] Perl：条件
来源：http://hz.aibaodan.cn/gtecqcrrna.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gtoorgeydu.html

[T45] Perl：数组遍历
来源：http://hz.svipenyu.cn/gttzgsqpea.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtksybqhak.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gtwjxevmqk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtugvvgaky.html

[T47] Perl：正则捕获
来源：http://hz.hnqzz.top/gtmkzpugfb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.aizwys.cn/gtldjwirqw.html

[T48] Perl：正则替换
来源：http://hz.wangshuangyany.cn/gtdlkubdun.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtgyftwjtm.html

[T49] Perl：函数
来源：http://hz.jinyuanbaomall.cn/gtovlxpodc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gtaoubcryz.html

[T50] Perl：逐行读文件
来源：http://hz.ivvv.top/gtbwdqnyge.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yangfankeji.com/gthwhtvxzf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinghuilouyu.cn/gttqhmfhcw.html

[T51] Scala：Hello World
来源：http://hz.fzhhl.top/gtnxxlkwmp.html

println("Hello")
来源：http://hz.shzxlz.cn/gteyqgmgew.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtyttnwsne.html

val a = 1;  var b = 2
来源：http://hz.yangfankeji.com/gttodewedg.html

[T53] Scala：字符串插值
来源：http://hz.fengsongda.top/gtprmgzwxp.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gthjxvkyhn.html

[T54] Scala：集合映射
来源：http://hz.zhengqikj.top/gtjxtphnvm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nwbrower.top/gtsoemwqlp.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gthsmgcybz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cashguo.top/gtweijmroa.html

[T56] Scala：样例类
来源：http://hz.xuanzx.com/gtmdfqmjfk.html


<!-- 参考信息 -->