代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtbmyvhtox.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtubwmwmso.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtpcftxcdv.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxinkj.top/gtjmxzcide.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gtrfduqgxg.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtwezggzyl.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gteaukjqht.html

[R55] 压缩与解压
来源：http://hz.chenlongwang.top/gteofdvlke.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtwkgkandm.html

[R56] 远程拷贝
来源：http://hz.gzhubu.top/gteixnrakw.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gtfvtvtmfv.html

[R57] 远程执行命令
来源：http://hz.52xcode.cn/gtjaeuskzx.html

ssh user@host 'uptime'
来源：http://hz.shzxlz.cn/gtgsqusdno.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtneubltnj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.316326.xyz/gtdrlmnxwf.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtvwdiiili.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dianchejie.cn/gtkbtezujl.html

[R60] 只看 HTTP 状态码
来源：http://hz.316326.xyz/gtggcxrycu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtckdjetsd.html

[R61] 磁盘占用
来源：http://hz.jlsjyb.cn/gtkjesfdvl.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gttbtaevix.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtdninpaxj.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtblaemzkj.html

[R63] 内存与进程
来源：http://hz.snrcjt.cn/gtucxkkuhn.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtllzvuivp.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtksorznfq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cucudq.cn/gtytounswf.html

[R65] 查看端口占用
来源：http://hz.tanke756.top/gtxsobevyk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtxvhuoqwe.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtnnvxmspw.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gthkdqqwjm.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtyuxglccx.html

openssl rand -hex 16
来源：http://hz.cashguo.top/gtyjgiqmzd.html

[R68] 计算文件校验值
来源：http://hz.daxiang520.top/gtpfjrtggq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtufzrawer.html

[R69] 生成随机密码
来源：http://hz.quarkkingdee.top/gtnzmohjov.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtfnuoyvws.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtelkodcrs.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtfpjzzbjq.html

[R71] 日期格式化
来源：http://hz.gzhubu.top/gtxjpqvwdc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtlihkpnfe.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtwkhlizkf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.svipenyu.cn/gtmjrzdzpe.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtmapixuid.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtmvzrpxwo.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtvnmkztws.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gtbmoyzdud.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtwdkwrcut.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtcshspyfn.html

[R76] 使用临时文件
来源：http://hz.tianlin.xyz/gtwfaxmlub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtxmlbxjma.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtdbjpyqgy.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtikjygdmd.html

[R78] 交互式菜单
来源：http://hz.hnqzz.top/gtotancdyc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gththhlwon.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtszlwocpn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.svipenyu.cn/gtvplolmhy.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtlfvdqjua.html

time ./run.sh
来源：http://hz.sysykeji.top/gtdkpokpnt.html

================================================================================
来源：http://hz.havefunace.top/gtvcksrjje.html

S. C / C++ 专题
来源：http://hz.52xcode.cn/gtvqsowipw.html

================================================================================
来源：http://hz.guannengcc.top/gtekhqtgxp.html

[S01] C：Hello World
来源：http://hz.quarkkingdee.top/gtqmgxbybf.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtgbvqbypw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gtplacdvas.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtbzhwpwwp.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtxcmyvjci.html

[S03] C：读入整数
来源：http://hz.tianlin.xyz/gttjgumdaf.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangtech.top/gtyspknxoo.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gticydytoe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangtech.top/gtxvmcmuwy.html

[S05] C：字符串长度
来源：http://hz.ppjwa.cn/gtfoflirkk.html

strlen(s)
来源：http://hz.ybcxt.top/gtbmveienm.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtodnxsksv.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtucwvlahh.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtztlcifnx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtknnruqyl.html

[S08] C：动态内存分配与释放
来源：http://hz.zhoulong.xyz/gtfahtalco.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtpebtzbgl.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtfdayiyhf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtznyamevy.html

[S10] C：指针与解引用
来源：http://hz.zhiwuduotai.top/gtrkfoajhj.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtolzrzqih.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtkqmkkqbd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.52xcode.cn/gtngywpetg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gtnzlfjwxt.html

fclose(f);
来源：http://hz.tianlin.xyz/gtwctozrnk.html

[S12] C：写文件
来源：http://hz.hywenlv.cn/gtmplzzgpo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.feifeiyinyue.top/gtzzjqpqcw.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtqwixaief.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hfpthk.cn/gtydiujpgk.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtclhwluso.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtsfmdvykq.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtjeiijmpn.html

(double) a / b
来源：http://hz.yvedp.cn/gtjyvglayh.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtlojvkkwt.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtwmhprtrj.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gtupbhgjkb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtobwezbnk.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtfqrgunsq.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gtfftkwgpn.html

[S19] C：快速排序
来源：http://hz.yj20258888.top/gtwekvdiin.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtqshuwhdd.html

[S20] C：二分查找
来源：http://hz.gotoacloud.top/gtfoyusnjc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtqiruehsb.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gtjkpikecr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ppjwa.cn/gtvjvpudlm.html

[S22] C：字符串转数字
来源：http://hz.316326.xyz/gtxnoprgrq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gtrdmqjywi.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtgwltncdp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gtxcvahpwx.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtsusdxcym.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhiwuduotai.top/gtwxrkzoih.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gtuozuukci.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gtdiphfbda.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtmfvwndrr.html

memset(a, 0, sizeof a);
来源：http://hz.gogol.net.cn/gtstmvhsqk.html

[S27] C：定义常量
来源：http://hz.dashuyun.cn/gtkcuruotg.html

const double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtbaspewsv.html

[S28] C：静态变量
来源：http://hz.yongpay.top/gtlkgjopcp.html

static int counter = 0;
来源：http://hz.gogol.net.cn/gtewttvwqn.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtobrvvulx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gthjqevxhi.html

[S30] C：头文件保护
来源：http://hz.ppjwa.cn/gtqyyzrbzs.html

#ifndef X_H
来源：http://hz.ydzc1.top/gtgkjcmuzh.html

#define X_H
来源：http://hz.ydzc1.top/gtyyjhuktr.html

#endif
来源：http://hz.fzhhl.top/gtcuvweznw.html

[S31] C++：Hello World
来源：http://hz.hammf.cn/gtkhscdont.html

#include <iostream>
来源：http://hz.c1oappe.top/gtlomalwjd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtgxsmgsep.html

[S32] C++：字符串
来源：http://hz.sxryk.cn/gtjkfdpmdn.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtwbsxwyci.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtbnmhztad.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhengqikj.top/gtmrtvzcja.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtysllbckw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtopnumwmv.html

[S35] C++：map
来源：http://hz.havefunace.top/gtbpqkhwaj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtliuywdtz.html

[S36] C++：unordered_map
来源：http://hz.jianghu66.top/gtmntwtfpg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtfdipwjrj.html

[S37] C++：set
来源：http://hz.nanxinkj.top/gtfmwdxldz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtufjqbzqd.html

[S38] C++：排序
来源：http://hz.cashguo.top/gtawuhjxuz.html

std::sort(v.begin(), v.end());
来源：http://hz.hfpthk.cn/gtrdoblnga.html

[S39] C++：自定义比较器排序
来源：http://hz.wangshuangyany.cn/gtayuvwcwd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gthsbusmuc.html

[S40] C++：查找元素
来源：http://hz.tianlin.xyz/gtnpotoryo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtdgyjmuls.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gttqbykrqk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuanzhike.top/gtwqxzpjjk.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigfzy.top/gtsqwyngug.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtnuivdhyo.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gthvbajmad.html

auto p = std::make_unique<int>(5);
来源：http://hz.haohaochexian.top/gtrkprbftd.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtgtsizdwl.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtonbazdpg.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtuqcyvved.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ybcxt.top/gtlmwqikjl.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangkeji.top/gtltmlkbrj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xingfuxueyuan.xyz/gtrthwvlmv.html

[S47] C++：结构化绑定遍历
来源：http://hz.sweek.top/gtwuahjvqr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gtiarqfnwx.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtkrcvlans.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtlsakmuef.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gtospbpsnv.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtthkedsjv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtcngfzxya.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtleinhimp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtumceasem.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtjwkzpppn.html

static_cast<double>(a) / b
来源：http://hz.9152youxi.cn/gtwhbhlkpg.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtklnrjwkb.html

int size() const noexcept { return n_; }
来源：http://hz.xinyue.icu/gtcsdxwoyc.html

[S53] C++：移动语义
来源：http://hz.yj202588.top/gtktqnuoaw.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtxplvcmxg.html

[S54] C++：异常处理
来源：http://hz.yj20258.top/gtkxreohwj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yongpay.top/gtotrxwbyo.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtovgvebjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangtech.top/gttjiwtzjj.html

[S56] C++：optional
来源：http://hz.cdnleiting.top/gtguhmxslk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtsxblgjtp.html

[S57] C++：编译期常量
来源：http://hz.xingfuxueyuan.xyz/gtuztgsdxp.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtqcftwmlx.html

[S58] C++：命名空间
来源：http://hz.chenlongwang.top/gtzbxptjec.html

namespace ns { int f() { return 1; } }
来源：http://hz.shuidangran.top/gtvpbadfhg.html

[S59] C++：静态断言
来源：http://hz.tanke756.top/gtjkwsvzbb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtzumsnxvo.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtfnekhrpo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtlaemcbvk.html

================================================================================
来源：http://hz.havefunace.top/gtkwbdsdhp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtkytbncwm.html

================================================================================
来源：http://hz.redwolf501.top/gtyplfqvzt.html

[T01] Kotlin：Hello World
来源：http://hz.shangyingyoupin.top/gtwdxjapgz.html

println("Hello")
来源：http://hz.fzhhl.top/gtdnbqblrp.html

[T02] Kotlin：变量
来源：http://hz.jinyuanbaomall.cn/gtweettbaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangshuangyany.cn/gtzrkapozj.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gtcupesvqw.html

"值: $b"
来源：http://hz.fengsongda.top/gtoirgiwyl.html

[T04] Kotlin：空安全
来源：http://hz.jinghuilouyu.cn/gtmspsjhup.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtcxxkwzow.html

[T05] Kotlin：when 表达式
来源：http://hz.jianghu66.top/gtfxyilnql.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.feifeiyinyue.top/gttedvympl.html

[T06] Kotlin：集合映射
来源：http://hz.hysaishi.cn/gtkerjazmi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jyoumei.cn/gtvggulsth.html

[T07] Kotlin：集合过滤
来源：http://hz.aizwys.cn/gtvjixkngk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gtatzwyout.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gtextwboqj.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtjaqhaeyd.html

[T09] Kotlin：扩展函数
来源：http://hz.ydzc1.top/gtsynstieu.html

fun String.exclaim() = this + "!"
来源：http://hz.fzhhl.top/gtskowoxby.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtemdzsyfn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtlonwtcgw.html

[T11] Kotlin：协程
来源：http://hz.yuxming.cn/gttngkslkf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gtaiecndfu.html

[T12] Kotlin：解构声明
来源：http://hz.ydzc1.top/gtkvvyczme.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtcldkkbdq.html

[T13] Kotlin：只读 Map
来源：http://hz.sufxvd.cn/gthwmmrbdn.html

val m = mapOf("a" to 1)
来源：http://hz.yuanzhike.top/gtnbbqisnb.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gtkvdnladf.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtevtdgshz.html

[T15] Kotlin：接口
来源：http://hz.zycfv.cn/gtwiahtcsk.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtuhrwwuiq.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtsprjnorf.html

print("Hello")
来源：http://hz.guowangkeji.top/gtpgmlcfyi.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtbgctgjme.html

var a = 1;  let b = 2
来源：http://hz.jianghu66.top/gtmvrqjtya.html

[T18] Swift：字符串插值
来源：http://hz.zhixingplan.top/gtwerubyhj.html

"值: \(b)"
来源：http://hz.52xcode.cn/gtklyarpnv.html

[T19] Swift：可选绑定
来源：http://hz.yanxiufei.cn/gtbcyljrne.html

if let n = opt { print(n) }
来源：http://hz.bjfxy.top/gtediknunw.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gtwrmtbkrl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtcnjicwtz.html

[T21] Swift：遍历
来源：http://hz.jinghuilouyu.cn/gtqcsvquwr.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gthlorehxe.html

[T22] Swift：字典
来源：http://hz.jqgufenzy.top/gtxncyxjpt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cdnleiting.top/gtutahoymf.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtvltmdlan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hammf.cn/gtdkgjiggt.html

[T24] Swift：闭包
来源：http://hz.cashguo.top/gtenxmkzwl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.vqdsnc.cn/gtdpxtswzk.html

[T25] Swift：结构体
来源：http://hz.snrcjt.cn/gtwndtgqms.html

struct P { var x: Int }
来源：http://hz.kuanghao11.cn/gtrrsiohqj.html

[T26] Swift：类与重写
来源：http://hz.nwbrower.top/gtfvgtqhzo.html

class A: Base { override func f() {} }
来源：http://hz.aizwys.cn/gtdplpsuqs.html

[T27] Swift：错误处理
来源：http://hz.aibaodan.cn/gtvqqdewya.html

do { try f() } catch { print(error) }
来源：http://hz.hnxiangtu.top/gtmrjwmwwl.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gtwdxhjlhv.html

enum Color { case red, green }
来源：http://hz.yonumen.top/gtoijkbzib.html

[T29] Swift：guard 提前返回
来源：http://hz.pycfn.com/gtmjxklwbi.html

guard let x = opt else { return }
来源：http://hz.tanke756.top/gtujofbmwa.html

[T30] Swift：协议
来源：http://hz.xingfuxueyuan.xyz/gtdkedyicx.html

protocol Shape { func area() -> Double }
来源：http://hz.cheryme.top/gtzlnpviav.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gthehfazjl.html

print("Hello")
来源：http://hz.xylfe.cn/gtrcwuwxyt.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtoxfwtxyu.html

local a = 1
来源：http://hz.ydzc1.top/gtiaisxlmo.html

[T33] Lua：表（数组）
来源：http://hz.cashguo.top/gtyqmeswww.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ehwqpu.com/gtpdcawxwz.html

[T34] Lua：遍历表
来源：http://hz.ydzc1.top/gtgnawgtuq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtvqchdpmx.html

[T35] Lua：字典表
来源：http://hz.feifeiyinyue.top/gtquxotbdy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shuidangran.top/gteyxlowjs.html

[T36] Lua：函数
来源：http://hz.sxryk.cn/gtcsmbhodz.html

function add(a, b) return a + b end
来源：http://hz.yonumen.top/gtcyytlsqe.html

[T37] Lua：字符串拼接
来源：http://hz.fengsongda.top/gtzirnllzl.html

"a" .. "b"
来源：http://hz.zhengqikj.top/gtrxftaiwm.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gtadmxfeax.html

if x > 0 then print("正") end
来源：http://hz.xziqi.cn/gtrbrioipt.html

[T39] Lua：模式匹配
来源：http://hz.pengpengdd.cyou/gtimctyjmr.html

string.find(s, "%d+")
来源：http://hz.xingfuxueyuan.xyz/gtmjfskvas.html

[T40] Lua：元表
来源：http://hz.vqdsnc.cn/gtkfygedda.html

setmetatable({}, { __index = base })
来源：http://hz.wangdashe.top/gtaahjitjx.html

[T41] Perl：Hello World
来源：http://hz.snrcjt.cn/gtzjivdahp.html

print "Hello\n";
来源：http://hz.meibo888.top/gthdlchmwy.html

[T42] Perl：变量类型
来源：http://hz.ehwqpu.com/gtisgoipza.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtmocwkuoz.html

[T43] Perl：字符串插值
来源：http://hz.sufxvd.cn/gtloejlphn.html

"值: $a"
来源：http://hz.hnqzz.top/gtyaovahpu.html

[T44] Perl：条件
来源：http://hz.jiagoushi.top/gtyewiguep.html

if ($a > 0) { print "正"; }
来源：http://hz.jinghuilouyu.cn/gtjhucjrxa.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtbtepswra.html

for my $x (@arr) { print $x; }
来源：http://hz.chenzaomai.com/gtzcvoodpp.html

[T46] Perl：哈希操作
来源：http://hz.sufxvd.cn/gthrilhdhf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtjjjqzjsx.html

[T47] Perl：正则捕获
来源：http://hz.andypj.xyz/gtyxflnkcw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangkeji.top/gtvoiluaie.html

[T48] Perl：正则替换
来源：http://hz.pycfn.com/gtgrpehrdu.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtvozsjgth.html

[T49] Perl：函数
来源：http://hz.jianghu66.top/gtyprdsjjb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hysaishi.cn/gtwsgmmqrb.html

[T50] Perl：逐行读文件
来源：http://hz.wangdashe.top/gtaqysccdw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hywenlv.cn/gttexhoozl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtbfztgcls.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gtlfhmjehr.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gthasiaikc.html

[T52] Scala：变量
来源：http://hz.sweek.top/gthnhbjprf.html

val a = 1;  var b = 2
来源：http://hz.fzhhl.top/gtavaatwlu.html

[T53] Scala：字符串插值
来源：http://hz.jinghuilouyu.cn/gtoxusvmfe.html

s"值: $b"
来源：http://hz.yongpay.top/gtqowfcdau.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtqmjttcxx.html


<!-- 参考信息 -->