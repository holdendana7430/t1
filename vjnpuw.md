代发 wailian999

cmd > out.log 2>&1
来源：http://hz.xziqi.cn/gtbemgnxji.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtitsrgwjh.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtvyffjjgl.html

[R41] 丢弃输出
来源：http://hz.zhoulong.xyz/gteupdpbvz.html

cmd >/dev/null 2>&1
来源：http://hz.ydjk.org.cn/gtfppurdwr.html

[R42] 输入重定向
来源：http://hz.zhaomingkeji.xyz/gtbqjllqwc.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtwycpxjko.html

[R43] 按名字查找文件
来源：http://hz.sweek.top/gtzuopdqlr.html

find . -name "*.log" -type f
来源：http://hz.mhx1999.top/gtqvqzgplh.html

[R44] 按修改时间查找
来源：http://hz.hongshengwenyu.top/gtzeybpqlm.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtvavovtbg.html

[R45] 批量删除
来源：http://hz.guowangkeji.top/gtkkjkpjhh.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gttnietiyv.html

[R46] 递归替换文件内容
来源：http://hz.zdqjudy.top/gtczwqznid.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gthefjllrg.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtyteyytcf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.c1oappe.top/gtipnxmmzz.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtcgjzehek.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gtfkdjrxri.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtinggjkhn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtyozzpnkv.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtnneaukig.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gthwhvscto.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gtjvjdcjme.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daria6918.cn/gtokdffejh.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtoskwufrj.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtpsdbfjjv.html

[R53] 查看文件头与实时尾
来源：http://hz.yuanzhike.top/gtaslvtoiw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtmhzbwxpn.html

[R54] 比较两个文件
来源：http://hz.cdnleiting.top/gtcreoxlum.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gtvcecrtxf.html

[R55] 压缩与解压
来源：http://hz.dashuyun.cn/gtzcookddf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guowangkeji.top/gtjfwltqej.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtrpmezozp.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gthmmesedc.html

[R57] 远程执行命令
来源：http://hz.quarkkingdee.top/gtprlouhrb.html

ssh user@host 'uptime'
来源：http://hz.xylfe.cn/gtlbuipmek.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtsbqkmqqc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.mhx1999.top/gtqmfnhrwm.html

[R59] 发 POST JSON
来源：http://hz.jiagoushi.top/gtdnhocyfb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtsasfprnu.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtwmpjcgkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj202588.top/gtkokrmwte.html

[R61] 磁盘占用
来源：http://hz.jinqigufen.top/gtvvpnqwsh.html

df -h;  du -sh *
来源：http://hz.52xcode.cn/gtfxniwtnp.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gtgkfltdic.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtuclluehs.html

[R63] 内存与进程
来源：http://hz.dianchejie.cn/gtirmnwrru.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtrhumfxor.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtiveqfsvl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gthnpevoye.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtdauwozxr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gtozcyzgpe.html

[R66] 定时任务
来源：http://hz.meibo888.top/gthwujojhz.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtqjklasbm.html

[R67] 生成随机十六进制串
来源：http://hz.zhoulong.xyz/gtqwdnephz.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtrxfsiiuz.html

[R68] 计算文件校验值
来源：http://hz.cqqwz.cn/gtuaatgkze.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigfzy.top/gtfmvhxxsk.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtajkvvlzz.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gtbmygfzvm.html

[R70] 时间戳与互转
来源：http://hz.sxryk.cn/gtgdfqpvle.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtxbimcgrh.html

[R71] 日期格式化
来源：http://hz.zycfv.cn/gtccuhrmbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtjinqwial.html

[R72] 等待端口就绪
来源：http://hz.yvedp.cn/gtblotmxrv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gzhubu.top/gtdyjnnttm.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtsmnhljbl.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtiylmvrkk.html

[R74] 批量重命名
来源：http://hz.jqgfzy.top/gtbpbrqsse.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuxming.cn/gtlrxkltst.html

[R75] 导出环境变量
来源：http://hz.smart0.xyz/gttkukjais.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zdqjudy.top/gtuiqujznz.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtqvfjwhxz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtoxladmcn.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtlumoytrd.html

read -rp "请输入: " ans
来源：http://hz.wangshuangyany.cn/gtmkxlkanh.html

[R78] 交互式菜单
来源：http://hz.yuanzhike.top/gtaphpauhd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pengpengdd.cyou/gttligmalf.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtpkxtiwpp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zycfv.cn/gtliggwtxp.html

[R80] 查看脚本执行耗时
来源：http://hz.snrcjt.cn/gtautsyzdc.html

time ./run.sh
来源：http://hz.xuanzx.com/gtjkntlpkv.html

================================================================================
来源：http://hz.aizwys.cn/gtggynrtzd.html

S. C / C++ 专题
来源：http://hz.zdqjudy.top/gtelzolmih.html

================================================================================
来源：http://hz.iojbl.cn/gtxclqjova.html

[S01] C：Hello World
来源：http://hz.guannengcc.top/gtghfdkklp.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gtvoehishq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtztqgiwsf.html

[S02] C：变量与格式化输出
来源：http://hz.guowangkeji.top/gtgdvjjagq.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtmtumxezt.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtqprubgfj.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtwturcjbg.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gtzjnrndpx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtgjouqpkq.html

[S05] C：字符串长度
来源：http://hz.guannengcc.top/gtkedsepfx.html

strlen(s)
来源：http://hz.ppjwa.cn/gtlcyfhsfc.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtnvgdenvo.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtyxsnxoeb.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtssqqavzd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtccqvzuue.html

[S08] C：动态内存分配与释放
来源：http://hz.shzxlz.cn/gtrwiikazr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gttbtmejbj.html

[S09] C：结构体定义与初始化
来源：http://hz.birdmap.top/gtlbosybqt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.redwolf501.top/gttixsyvlu.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtnyoifgfz.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gtzggfupqv.html

[S11] C：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtyurxvtyu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tianlin.xyz/gtdbeznhiw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtgmaxggjg.html

fclose(f);
来源：http://hz.cqqwz.cn/gthapaagfr.html

[S12] C：写文件
来源：http://hz.xuanzx.com/gtfnewjxzr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.smart0.xyz/gtazcrjxsq.html

[S13] C：宏定义
来源：http://hz.iojbl.cn/gthwyektyy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gtrmeftwpy.html

[S14] C：枚举
来源：http://hz.mhx1999.top/gtgdhvgguo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtrddyqoja.html

[S15] C：类型转换
来源：http://hz.yongpay.top/gtrsvrjcgy.html

(double) a / b
来源：http://hz.xinyue.icu/gtwkjhhsnd.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtxiaxyuxm.html

x |= (1 << 3);
来源：http://hz.aizwys.cn/gtdxfqdgaz.html

[S17] C：安全拼接字符串
来源：http://hz.yvedp.cn/gtvzwrysrd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtiefxivqc.html

[S18] C：命令行参数
来源：http://hz.xziqi.cn/gtopzoqcpr.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtahnffnbq.html

[S19] C：快速排序
来源：http://hz.daxiang520.top/gtlteikswk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gttabzfwsy.html

[S20] C：二分查找
来源：http://hz.jianghu66.top/gtrflmguqf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtehbjrkjp.html

[S21] C：字符类别判断
来源：http://hz.hnqzz.top/gtkspybcun.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtaknpoiwh.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtybkbcxcq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.redwolf501.top/gtribflpvi.html

[S23] C：随机数
来源：http://hz.jqgfzy.top/gtimhrbuhq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtlwtijnfm.html

[S24] C：获取本地时间
来源：http://hz.yuxming.cn/gtycfvyerr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtuotofgzq.html

[S25] C：内存拷贝
来源：http://hz.yueranfly.top/gtieubrwsa.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtmkbookbz.html

[S26] C：内存清零
来源：http://hz.yueranfly.top/gtwxlnqdcp.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gtdmgxvldf.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtuwdpdupx.html

const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtgbfelfxv.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtwktjdlou.html

static int counter = 0;
来源：http://hz.jinqigfzy.top/gtnrbyzgxg.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtgzjsgvza.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gtumlmbcox.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtdkmkrmnq.html

#ifndef X_H
来源：http://hz.daria6918.cn/gtzdnbgyip.html

#define X_H
来源：http://hz.hnxiangtu.top/gtxkqlyfzl.html

#endif
来源：http://hz.fzhhl.top/gtoidhmjwh.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtrixzilct.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtwrrpdygv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gteprjrtai.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtclzjdmmk.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gttpgnouhj.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtvpxbihwv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtkwhksdcp.html

[S34] C++：遍历 vector
来源：http://hz.jlsjyb.cn/gtwqhnxmbs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtdeyllcbv.html

[S35] C++：map
来源：http://hz.pycfn.com/gtezejywic.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtiewwuwus.html

[S36] C++：unordered_map
来源：http://hz.c1oappe.top/gtcugrfeyr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtjksfcrui.html

[S37] C++：set
来源：http://hz.pengpengdd.cyou/gtlytjegyq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtfzdwmdkt.html

[S38] C++：排序
来源：http://hz.zhoulong.xyz/gtxwsfjvjc.html

std::sort(v.begin(), v.end());
来源：http://hz.jyoumei.cn/gtbjnmodyp.html

[S39] C++：自定义比较器排序
来源：http://hz.fzhhl.top/gtxcrvwhyk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtbtfzicvm.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtnmkogaaa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtnntutgqu.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gttnzbxnkw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtkriadvto.html

[S42] C++：继承与虚函数
来源：http://hz.gaohongyu789.top/gtntpgelrh.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtvccmwlzs.html

[S43] C++：智能指针
来源：http://hz.redwolf501.top/gtrmbvvsbr.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtkkndeqkp.html

[S44] C++：引用传参
来源：http://hz.yangfankeji.com/gtevhmxyoi.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtmbptejia.html

[S45] C++：lambda
来源：http://hz.ydjk.org.cn/gtmhcntadr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtjtjlbfzf.html

[S46] C++：函数模板
来源：http://hz.ydzc1.top/gtityzaqhr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cheryme.top/gtxecfirjt.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinghuilouyu.cn/gtulawygqi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtjutgultg.html

[S48] C++：逐行读文件
来源：http://hz.yanxiufei.cn/gtvhynzmpj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtjacvftaw.html

while (std::getline(in, line)) { }
来源：http://hz.yonumen.top/gtjnizwifb.html

[S49] C++：写文件
来源：http://hz.hongshengwenyu.top/gtjzunqvts.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gthiekwetv.html

[S50] C++：格式化数字
来源：http://hz.cashguo.top/gtzqfotyqz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.quarkkingdee.top/gtnbfuvwup.html

[S51] C++：显式类型转换
来源：http://hz.smart0.xyz/gtbjsofqzy.html

static_cast<double>(a) / b
来源：http://hz.zhoulong.xyz/gtdachbsjb.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtciapjdgb.html

int size() const noexcept { return n_; }
来源：http://hz.kuanghao11.cn/gthdeuyjlt.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtlngfptlf.html

std::vector<int> w = std::move(v);
来源：http://hz.chenlongwang.top/gterdntycd.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gttptmzglt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtottvuzpb.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtqzcpzkak.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtvvgopmyb.html

[S56] C++：optional
来源：http://hz.guannengcc.top/gtuebsjcmk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ppjwa.cn/gtewfjdpit.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtkimtlniu.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gtsrlrxfej.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtmxeubaio.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtufdfxair.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtuacheddw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhiwuduotai.top/gtvozbielf.html

[S60] C++：遍历并删除元素
来源：http://hz.pycfn.com/gtabqabsgw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtsaghuqni.html

================================================================================
来源：http://hz.haohaochexian.top/gtrdlmzhln.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.smart0.xyz/gtgkucnluv.html

================================================================================
来源：http://hz.ivvv.top/gtkobjqpqz.html

[T01] Kotlin：Hello World
来源：http://hz.zdqjudy.top/gtraioknis.html

println("Hello")
来源：http://hz.sxryk.cn/gtjrtyrijo.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtdqekbixs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gtvcqqepws.html

[T03] Kotlin：字符串模板
来源：http://hz.yangfankeji.com/gtesnafrsx.html

"值: $b"
来源：http://hz.hongshengwenyu.top/gtotbyhhkx.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gtrqnoqkdk.html

val n: String? = null;  n?.length
来源：http://hz.smart0.xyz/gtvaotsvin.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gtuplcnrdm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pycfn.com/gtsjbmewvy.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtpnazlijn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gogol.net.cn/gtjuyrmpna.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtaovbsyff.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtmjlwrdkx.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gtmnuwmoih.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtlcxvbiyu.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxinkj.top/gtafabzdnf.html

fun String.exclaim() = this + "!"
来源：http://hz.xziqi.cn/gtvsrsnpxl.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtajykrggo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.havefunace.top/gtijwtuvwe.html

[T11] Kotlin：协程
来源：http://hz.snrcjt.cn/gtisekndav.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xingfuxueyuan.xyz/gtpxcffivt.html

[T12] Kotlin：解构声明
来源：http://hz.fengsongda.top/gtqskhapbk.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtgojogzwt.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtyhfpttmi.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtrdadaujc.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtklzmtpcc.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtsypamedb.html

[T15] Kotlin：接口
来源：http://hz.chenjidiqi.icu/gtxkynhmff.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtqgcelgsf.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gttfbyufeu.html

print("Hello")
来源：http://hz.yj20258.top/gtuzprapmc.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gthzfwmead.html

var a = 1;  let b = 2
来源：http://hz.aizwys.cn/gtcrlxeort.html

[T18] Swift：字符串插值
来源：http://hz.gogol.net.cn/gtyscedzvu.html

"值: \(b)"
来源：http://hz.fengsongda.top/gterqcvwqx.html

[T19] Swift：可选绑定
来源：http://hz.jinqigufen.top/gtmzjbfkhj.html

if let n = opt { print(n) }
来源：http://hz.meibo888.top/gtyrucmlje.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtehrzehwu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.kuanghao11.cn/gttwqrijoq.html

[T21] Swift：遍历
来源：http://hz.nwbrower.top/gtkniyjxcv.html

for x in a { print(x) }
来源：http://hz.jyoumei.cn/gthsanuweu.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtmtcecyva.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hammf.cn/gtcqsexkso.html

[T23] Swift：函数
来源：http://hz.hnxiangtu.top/gtgqoeflzg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtldfhpggz.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtzverjeek.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daria6918.cn/gtmunippia.html

[T25] Swift：结构体
来源：http://hz.guowangkeji.top/gtjlapjjdl.html

struct P { var x: Int }
来源：http://hz.sysykeji.top/gtaatftpiz.html

[T26] Swift：类与重写
来源：http://hz.316326.xyz/gtfdvpckej.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtdeaukmka.html

[T27] Swift：错误处理
来源：http://hz.bjfxy.top/gtzukqisda.html

do { try f() } catch { print(error) }
来源：http://hz.0kj1m.cn/gtrxpcndbk.html

[T28] Swift：枚举
来源：http://hz.yonumen.top/gtzkuulgys.html

enum Color { case red, green }
来源：http://hz.haohaochexian.top/gtyihukabd.html

[T29] Swift：guard 提前返回
来源：http://hz.yueranfly.top/gtrpfnjcsz.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtsrdfhcnd.html

[T30] Swift：协议
来源：http://hz.iojbl.cn/gtchfspuvy.html

protocol Shape { func area() -> Double }
来源：http://hz.ydzc1.top/gtqvmsswtq.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtveatxytw.html

print("Hello")
来源：http://hz.hywenlv.cn/gtrltvhbnf.html

[T32] Lua：局部变量
来源：http://hz.xziqi.cn/gthunphypa.html

local a = 1
来源：http://hz.zhongyouzk.top/gtkvweovmp.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtwflymnjw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.bjfxy.top/gtbcywcptx.html

[T34] Lua：遍历表
来源：http://hz.tian-w.cn/gtobxeakgp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtxmdpqekw.html

[T35] Lua：字典表
来源：http://hz.jiagoushi.top/gtcbwrsybi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tian-w.cn/gtwhfzlbvu.html

[T36] Lua：函数
来源：http://hz.yuxming.cn/gtslawrbeh.html

function add(a, b) return a + b end
来源：http://hz.zhixingplan.top/gtfvrfnovy.html

[T37] Lua：字符串拼接
来源：http://hz.zhijiandao.cn/gtiyfmibkm.html

"a" .. "b"
来源：http://hz.zhoulong.xyz/gthwxztpxi.html

[T38] Lua：条件
来源：http://hz.hnqzz.top/gtvgtwzsxo.html

if x > 0 then print("正") end
来源：http://hz.hfpthk.cn/gtzshffpce.html

[T39] Lua：模式匹配
来源：http://hz.meibo888.top/gtzwzxrcyl.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtidmgnscc.html

[T40] Lua：元表
来源：http://hz.zhaomingkeji.xyz/gtsqcgdbse.html

setmetatable({}, { __index = base })
来源：http://hz.gaohongyu789.top/gtnimjrqbw.html

[T41] Perl：Hello World
来源：http://hz.chenzaomai.com/gtgyhmllou.html

print "Hello\n";
来源：http://hz.xinyue.icu/gtwsaruatb.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtyctkaajv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gtlopmtnlj.html


<!-- 参考信息 -->