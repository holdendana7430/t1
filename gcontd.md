代发 wailian999

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gtvukpoxjv.html

[R40] 追加写日志
来源：http://hz.shuidangran.top/gteebamoof.html

echo "log" >> out.log
来源：http://hz.cqqwz.cn/gtgancbuuy.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtgvurnrig.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigfzy.top/gtckvqtvbt.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtlmtioqkw.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtaxufkojy.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gtwsusjqae.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtjjeyyqii.html

[R44] 按修改时间查找
来源：http://hz.zycfv.cn/gtsqhfbzqn.html

find . -mtime -7 -type f
来源：http://hz.aibaodan.cn/gtuqydlnpy.html

[R45] 批量删除
来源：http://hz.nanxinkj.top/gtvdgchyxf.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtgkxdupur.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gtvbbdtknb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtrjfktfkd.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtnebquixs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.kuanghao11.cn/gtbxlgxbhn.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtodzxydcs.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtujkocofj.html

[R49] awk 带条件
来源：http://hz.zhiwuduotai.top/gthxsnzmyc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnqzz.top/gtxjqypqwr.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtembpfpmf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtzgcxjjau.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtcnnelvvn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gtfvrmuysx.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gthycznkmh.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtmdiyatig.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtwlnpeghn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.vqdsnc.cn/gthtmuzbiq.html

[R54] 比较两个文件
来源：http://hz.sysykeji.top/gtdgwzcylg.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtdrjptjae.html

[R55] 压缩与解压
来源：http://hz.hnxiangtu.top/gtlsxzvrqr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gtltnopiac.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtaphiwqhy.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtboyirqqs.html

[R57] 远程执行命令
来源：http://hz.hongshengwenyu.top/gtbyswvrcy.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtzlawirgy.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtznsafkea.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ehwqpu.com/gtrtnxdsfi.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtdwmhszxj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hongshengwenyu.top/gtsklqysqz.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtkpszssrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtocuvungk.html

[R61] 磁盘占用
来源：http://hz.ywan-chungtsiang.top/gtliajukjf.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gtxtpcfiex.html

[R62] 找最占空间的文件
来源：http://hz.jlsjyb.cn/gtgzyagtio.html

du -ah . | sort -rh | head -10
来源：http://hz.snrcjt.cn/gtyiyfekgy.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtcxevhobo.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtvfmvwusi.html

[R64] 结束进程
来源：http://hz.hywenlv.cn/gtsnqylnjg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cqqwz.cn/gtemmagwbn.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtsiiwafni.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtcgjnbvgw.html

[R66] 定时任务
来源：http://hz.cdnleiting.top/gtelvljmqi.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtbsnwzdgs.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtwwktqpyv.html

openssl rand -hex 16
来源：http://hz.zhixingplan.top/gtrqvxihkm.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gthxorsdga.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fengsongda.top/gtqrotfxxg.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gthkdlffep.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtygzqonka.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gttgmdkztr.html

date +%s;  date -d @1700000000
来源：http://hz.cqqwz.cn/gtzzeroezh.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtdhwbvcun.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtnbbznpix.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtflluvtfx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtdxqdqiue.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtonekqbhu.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtnueyoazi.html

[R74] 批量重命名
来源：http://hz.daria6918.cn/gtzbflrydm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtcsiseouu.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtwonnmmsa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnqzz.top/gtfduzglcg.html

[R76] 使用临时文件
来源：http://hz.c1oappe.top/gtzewxbzxm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtciekslky.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtowhanjuo.html

read -rp "请输入: " ans
来源：http://hz.sysykeji.top/gtxxgbkfgl.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtiboxngts.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtbgmhzltn.html

[R79] 解析命令行选项
来源：http://hz.guannengcc.top/gtflczdwwe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtqtxjknog.html

[R80] 查看脚本执行耗时
来源：http://hz.shzxlz.cn/gtqrmescnf.html

time ./run.sh
来源：http://hz.ydjk.org.cn/gtdwhnrtko.html

================================================================================
来源：http://hz.smart0.xyz/gtuwurfopv.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gttnqpfshd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvkxayzap.html

[S01] C：Hello World
来源：http://hz.feifeiyinyue.top/gtxpjufcqr.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtorvfqhws.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangtech.top/gtoahxvvyk.html

[S02] C：变量与格式化输出
来源：http://hz.zhijiandao.cn/gtoklsshpg.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtavqrtxoz.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtwawumber.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtikfvcewn.html

[S04] C：字符串复制
来源：http://hz.guannengcc.top/gtemzgsyem.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtgkayvqhm.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtepqptcxr.html

strlen(s)
来源：http://hz.jiagoushi.top/gtbuvcurqw.html

[S06] C：字符串比较
来源：http://hz.jqgfzy.top/gtkcsqzlij.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtapfouzgk.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtgvnuwjzh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.bjfxy.top/gtqkjelchz.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtevpftzww.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtfjdampid.html

[S09] C：结构体定义与初始化
来源：http://hz.cheryme.top/gtkrobqnuu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtivocbcxy.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtiuotcuqi.html

int *p = &a;  *p = 5;
来源：http://hz.ywan-chungtsiang.top/gtengwdihw.html

[S11] C：逐行读文件
来源：http://hz.quarkkingdee.top/gtrezbknph.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtogcovrnc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtlywxgwwk.html

fclose(f);
来源：http://hz.tanke756.top/gttenoxcju.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtemvmbyxw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtbakubtnc.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gthmbommnb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtvhzrhpkd.html

[S14] C：枚举
来源：http://hz.cqqwz.cn/gtilwraxyd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gttbuswemg.html

[S15] C：类型转换
来源：http://hz.hysaishi.cn/gtfgsblkeg.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtrkyzaklc.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtbabwkhlc.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtwtogtrod.html

[S17] C：安全拼接字符串
来源：http://hz.tian-w.cn/gtunkqejqq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fzhhl.top/gtqczhvztv.html

[S18] C：命令行参数
来源：http://hz.xuanzx.com/gtupnibcha.html

int main(int argc, char **argv)
来源：http://hz.xingfuxueyuan.xyz/gtsamjxtdr.html

[S19] C：快速排序
来源：http://hz.jlsjyb.cn/gtgphsnkch.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtrdfptzoo.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtczabjomx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtfllpvatc.html

[S21] C：字符类别判断
来源：http://hz.chenlongwang.top/gtmyhxadru.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gtdjynzbhb.html

[S22] C：字符串转数字
来源：http://hz.birdmap.top/gtbtlljolm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtxkpieqsx.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtoffwfkxc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtxykjnfbf.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtbwsvjesm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shzxlz.cn/gtwnghismp.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtxpeqkfuq.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtzapsmaef.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtkeolmize.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtmugsawfa.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtbbgogqfl.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtqwknnamu.html

[S28] C：静态变量
来源：http://hz.shanyushiyangtech.top/gtnnemvqqq.html

static int counter = 0;
来源：http://hz.ivvv.top/gtrsurggtx.html

[S29] C：变参函数
来源：http://hz.xinyue.icu/gtazfbiqas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.bjfxy.top/gthyuerunb.html

[S30] C：头文件保护
来源：http://hz.ydjk.org.cn/gtpgrcinjk.html

#ifndef X_H
来源：http://hz.mhx1999.top/gtrhmtfrde.html

#define X_H
来源：http://hz.haohaochexian.top/gtlxpcdkrn.html

#endif
来源：http://hz.jinqigfzy.top/gtggmfagpm.html

[S31] C++：Hello World
来源：http://hz.zhiwuduotai.top/gtxhatemie.html

#include <iostream>
来源：http://hz.aizwys.cn/gtlpdtgmrw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xylfe.cn/gtjwynditc.html

[S32] C++：字符串
来源：http://hz.fzhhl.top/gtynyqirsx.html

std::string s = "hi";  s += "!";
来源：http://hz.havefunace.top/gtrpwdizta.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtkbvstqfx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtdamgdrql.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtiynehnso.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtqkuhyqnm.html

[S35] C++：map
来源：http://hz.zdqjudy.top/gtjbmyjome.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtghxeuqww.html

[S36] C++：unordered_map
来源：http://hz.guowangkeji.top/gtyawgzeoe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtykmaszrp.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtroqgecdu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhengqikj.top/gtekhgqsiy.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtvsorbgbb.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gtruxhzlel.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtoaeltkqu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtnvpddqrv.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gthyuklsoe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtcnwdqkxa.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gtbpgfvkjv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gttnkstkuy.html

[S42] C++：继承与虚函数
来源：http://hz.birdmap.top/gtjgdhoacv.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtrxoekkag.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtfapxkrof.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtzgpqjlzu.html

[S44] C++：引用传参
来源：http://hz.gaohongyu789.top/gtsquiuxvp.html

void inc(int &x) { ++x; }
来源：http://hz.chenlongwang.top/gtyteazten.html

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtnkdptsiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.svipenyu.cn/gtlmredjgq.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtotdgygtk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtocaiwulv.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuxming.cn/gtriqdbvxz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtlgisluvp.html

[S48] C++：逐行读文件
来源：http://hz.yonumen.top/gtiarnvewk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtvqoquvbv.html

while (std::getline(in, line)) { }
来源：http://hz.zhijiandao.cn/gtwvfurjxm.html

[S49] C++：写文件
来源：http://hz.wangdashe.top/gttpclcakj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258.top/gtsydltrxa.html

[S50] C++：格式化数字
来源：http://hz.jinghuilouyu.cn/gtfenxmspj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cucudq.cn/gttbubcxay.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtvmsoghqq.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtwguqwjqn.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtkgodgxnn.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtjfezzdoc.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtvfczutpr.html

std::vector<int> w = std::move(v);
来源：http://hz.hfpthk.cn/gtykiubeyn.html

[S54] C++：异常处理
来源：http://hz.cucudq.cn/gtjnplikpz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tianlin.xyz/gtemqugxis.html

[S55] C++：结构化绑定
来源：http://hz.chenlongwang.top/gtvnngqxed.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xinyue.icu/gtmdnkkuef.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtuhiemvhu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gtapjcewwp.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtljwakdgl.html

constexpr int N = 10;
来源：http://hz.gaohongyu789.top/gtofuvpzgm.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtdznuenrk.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gttovnxhle.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtwezghtqh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gtwajhcqzm.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtdkkzdvxb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xylfe.cn/gtoiurevam.html

================================================================================
来源：http://hz.ivvv.top/gtjykdvezr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtmhfbijib.html

================================================================================
来源：http://hz.nanxuanxn.top/gtysfpmunm.html

[T01] Kotlin：Hello World
来源：http://hz.tanke756.top/gtqihpxjch.html

println("Hello")
来源：http://hz.shzxlz.cn/gtbdxriosv.html

[T02] Kotlin：变量
来源：http://hz.c1oappe.top/gtgvzqwmaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtnqyfvfws.html

[T03] Kotlin：字符串模板
来源：http://hz.gzhubu.top/gtmutksrrp.html

"值: $b"
来源：http://hz.c1oappe.top/gtqghdjlrd.html

[T04] Kotlin：空安全
来源：http://hz.9152youxi.cn/gttcsryrnm.html

val n: String? = null;  n?.length
来源：http://hz.quarkkingdee.top/gtsuiqoojv.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtjqvcifng.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cqqwz.cn/gtjiarzben.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtisnukyif.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gtfalgefds.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtpytmuzsj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ehwqpu.com/gtrqqwctod.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtncqukfix.html

data class User(val name: String, val age: Int)
来源：http://hz.xuanzx.com/gtecukxbjn.html

[T09] Kotlin：扩展函数
来源：http://hz.ydzc1.top/gtslftmslk.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtidxfdrdu.html

[T10] Kotlin：默认参数
来源：http://hz.jqgfzy.top/gtswgidlzb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtusmohjyx.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtgxuuyniy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.havefunace.top/gtuqujduft.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtlihnhbwm.html

val (a, b) = Pair(1, 2)
来源：http://hz.tian-w.cn/gtdicrzxrl.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtbkymroan.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gtqaoaypkg.html

[T14] Kotlin：循环
来源：http://hz.vqdsnc.cn/gtpqbsxvjd.html

for (i in 1..10) println(i)
来源：http://hz.yanxiufei.cn/gtakqkgwxg.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtlwmhdmtp.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtumkykqqn.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtpkpkgigp.html

print("Hello")
来源：http://hz.yangfankeji.com/gtfmuqvuva.html

[T17] Swift：变量与常量
来源：http://hz.sufxvd.cn/gtxdquegwq.html

var a = 1;  let b = 2
来源：http://hz.quarkkingdee.top/gtyxnoyysv.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtcjtgxswf.html

"值: \(b)"
来源：http://hz.daxiang520.top/gtolgekqfa.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gtulqkwnpn.html

if let n = opt { print(n) }
来源：http://hz.zhijiandao.cn/gtbsgcgsmj.html

[T20] Swift：数组操作
来源：http://hz.jqgufenzy.top/gtikmmybku.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtogrkgtfn.html

[T21] Swift：遍历
来源：http://hz.cqqwz.cn/gtsoqkyctn.html

for x in a { print(x) }
来源：http://hz.jiagoushi.top/gtmbjribot.html

[T22] Swift：字典
来源：http://hz.chenlongwang.top/gtnjmfwpqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dianchejie.cn/gthudqaatu.html

[T23] Swift：函数
来源：http://hz.nanxuanxn.top/gttswukgfh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtwaczihya.html

[T24] Swift：闭包
来源：http://hz.sxryk.cn/gtjsuuaitn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhoulong.xyz/gternxlxpt.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtfuylhimz.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtcpykdfcs.html

[T26] Swift：类与重写
来源：http://hz.sxryk.cn/gtrguecbnk.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtvsxfodyq.html

[T27] Swift：错误处理
来源：http://hz.xylfe.cn/gtyogxpdaa.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtbkegrert.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtbgqcybbt.html

enum Color { case red, green }
来源：http://hz.0kj1m.cn/gtunaqscct.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtskwpxvso.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtpqdtqzfq.html

[T30] Swift：协议
来源：http://hz.gogol.net.cn/gthbqfrisk.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtpnwxytrt.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gtzmhrtyay.html

print("Hello")
来源：http://hz.xuanzx.com/gtomofoelz.html

[T32] Lua：局部变量
来源：http://hz.jinyuanbaomall.cn/gtwtebhfvt.html

local a = 1
来源：http://hz.xziqi.cn/gtypbhbmim.html

[T33] Lua：表（数组）
来源：http://hz.zhixingplan.top/gtmhnurogt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shangyingyoupin.top/gtomacmfcw.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtnhlnszid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenzaomai.com/gtbfkbuaas.html

[T35] Lua：字典表
来源：http://hz.quarkkingdee.top/gthgrrybqk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shuidangran.top/gtgmxqtdvz.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtwrtnfxhs.html

function add(a, b) return a + b end
来源：http://hz.cucudq.cn/gtpgabbimv.html

[T37] Lua：字符串拼接
来源：http://hz.jqgufenzy.top/gtkxiqahne.html

"a" .. "b"
来源：http://hz.gogol.net.cn/gthgmqbgto.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtiyvkxbfx.html

if x > 0 then print("正") end
来源：http://hz.yvedp.cn/gtuunvkusl.html

[T39] Lua：模式匹配
来源：http://hz.ydjk.org.cn/gternmlrbm.html

string.find(s, "%d+")
来源：http://hz.tian-w.cn/gtginrhaps.html

[T40] Lua：元表
来源：http://hz.daria6918.cn/gtlarkqvyz.html

setmetatable({}, { __index = base })
来源：http://hz.pycfn.com/gtuuvayuzr.html

[T41] Perl：Hello World
来源：http://hz.yuxming.cn/gtbqbsktac.html

print "Hello\n";
来源：http://hz.jianghu66.top/gttefgqllh.html

[T42] Perl：变量类型
来源：http://hz.yj20258888.top/gtdehpixws.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gtoidkpaqw.html


<!-- 参考信息 -->