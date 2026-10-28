代发 wailian999

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtyynzuamo.html

[R40] 追加写日志
来源：http://hz.guowangkeji.top/gtwvbdydqi.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtqkguuomk.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtgjoskcqi.html

cmd >/dev/null 2>&1
来源：http://hz.andypj.xyz/gtqimjzkhg.html

[R42] 输入重定向
来源：http://hz.hnxiangtu.top/gtpumexiny.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtqmslcqip.html

[R43] 按名字查找文件
来源：http://hz.hongshengwenyu.top/gtfodioxii.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtxvylmaco.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtfezcodtt.html

find . -mtime -7 -type f
来源：http://hz.yangfankeji.com/gtkzjyxmco.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gtijuvkvvq.html

find . -name "*.tmp" -delete
来源：http://hz.nanxinkj.top/gtpqbxekvd.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtaorwifvi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yongpay.top/gtsbxxidrt.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtaoopgzzx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ehwqpu.com/gtubnmwuew.html

[R48] awk 取指定列
来源：http://hz.haohaochexian.top/gtyosyptmc.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtdrcnxxdx.html

[R49] awk 带条件
来源：http://hz.xylfe.cn/gttyzxjhrn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guowangkeji.top/gthniuvhpd.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gtvvpysjrc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtnqlkpfgd.html

[R51] 排序去重取前几
来源：http://hz.chenlongwang.top/gtwhgplgep.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yueranfly.top/gtuwbvgtbq.html

[R52] 统计行数
来源：http://hz.hnxiangtu.top/gtsgyeroab.html

wc -l a.txt
来源：http://hz.xuanzx.com/gtmpsysnqn.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtjddcdfqa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtijgibseb.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gthcicnvsq.html

diff a.txt b.txt
来源：http://hz.bjfxy.top/gtlxthxgvh.html

[R55] 压缩与解压
来源：http://hz.xuetiantiany.cn/gtzjzluoso.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtohdwzlfg.html

[R56] 远程拷贝
来源：http://hz.havefunace.top/gtcberhzie.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtjxupxppr.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtfxyalvoz.html

ssh user@host 'uptime'
来源：http://hz.0kj1m.cn/gtengixybc.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gtlvcrhoyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtkichwajb.html

[R59] 发 POST JSON
来源：http://hz.316326.xyz/gtduibapxj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tanke756.top/gtbqxshtlp.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtcpjvowea.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj202588.top/gtjmrfpaqr.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gtqvrbpfar.html

df -h;  du -sh *
来源：http://hz.nanxuanxn.top/gtcvzdmvwu.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtkgbaftot.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtnqxwgsrm.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtfqvuhmqa.html

free -h;  ps aux | grep nginx
来源：http://hz.guannengcc.top/gtcodcfdzd.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtlrrmbzfy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtjpmucrba.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gtmmhsxejd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cdnleiting.top/gtjmgafesm.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtxmraqhaq.html

crontab -e;  crontab -l
来源：http://hz.cdnleiting.top/gtknlcioxi.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gtocuuvosj.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtzxpvyyro.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtloebyrjn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtorxsjbiw.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtmibeorow.html

head -c 16 /dev/urandom | base64
来源：http://hz.cashguo.top/gtlycejejm.html

[R70] 时间戳与互转
来源：http://hz.c1oappe.top/gtbulnrxed.html

date +%s;  date -d @1700000000
来源：http://hz.ydzc1.top/gtehglxhms.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtjegvlxnr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtrculgcmq.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtxwtwrxnp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtissgwbob.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gteltamiqh.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtlgqqbewo.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtekkkjvgf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtytgkhfzc.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gtomvboucd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.mhx1999.top/gtcqrdgbaj.html

[R76] 使用临时文件
来源：http://hz.xylfe.cn/gtbmgrjqko.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtfygkwmsd.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtrmolxoyp.html

read -rp "请输入: " ans
来源：http://hz.nanxuanxn.top/gtcyxwjrar.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtlmuugsqo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fengsongda.top/gtnbsytoel.html

[R79] 解析命令行选项
来源：http://hz.yongpay.top/gtzatfgxzb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hammf.cn/gtvdqckfen.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258.top/gtttdmsszc.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtpbqgahwg.html

================================================================================
来源：http://hz.gogol.net.cn/gtdvltwjao.html

S. C / C++ 专题
来源：http://hz.chenjidiqi.icu/gtsehidwqm.html

================================================================================
来源：http://hz.wangdashe.top/gtvhgpoqkl.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtssfwporr.html

#include <stdio.h>
来源：http://hz.ppjwa.cn/gtzxteqxck.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangshuangyany.cn/gtdqgbedqr.html

[S02] C：变量与格式化输出
来源：http://hz.ehwqpu.com/gtcntfnyih.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtmlciviif.html

[S03] C：读入整数
来源：http://hz.tian-w.cn/gtwlytvpsf.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtwpwczout.html

[S04] C：字符串复制
来源：http://hz.gaohongyu789.top/gtvadoyxkm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtblgizgbb.html

[S05] C：字符串长度
来源：http://hz.zycfv.cn/gttyxahdnf.html

strlen(s)
来源：http://hz.tianlin.xyz/gtojnjoari.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtjrpobgig.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gtqdrsxijw.html

[S07] C：数组遍历求和
来源：http://hz.dashuyun.cn/gtehrwucok.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cucudq.cn/gttggcjjzk.html

[S08] C：动态内存分配与释放
来源：http://hz.haohaochexian.top/gtyyobpkvy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtdharavdc.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gtxodvnorn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jyoumei.cn/gtvjvbboik.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtvdoeajze.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtvrtplsea.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtizdcjcgf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinyuanbaomall.cn/gtzhopukvz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.quarkkingdee.top/gtevyddvfe.html

fclose(f);
来源：http://hz.meibo888.top/gtcldnnjxg.html

[S12] C：写文件
来源：http://hz.daxiang520.top/gtlxlinzgw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shzxlz.cn/gtrojuvavr.html

[S13] C：宏定义
来源：http://hz.shanyushiyangtech.top/gthaitaoaj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtkdsbxnub.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gttgwyvtjq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gthdgpsucs.html

[S15] C：类型转换
来源：http://hz.9152youxi.cn/gtclugwtep.html

(double) a / b
来源：http://hz.meibo888.top/gtkylswwdi.html

[S16] C：位操作置位
来源：http://hz.nanxinkj.top/gtknziypmc.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtspnzqfkp.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtxbwhlaap.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtcgczptet.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtcgqgvbeh.html

int main(int argc, char **argv)
来源：http://hz.cucudq.cn/gtlboypqnv.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtankatcac.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtfrhjwwvx.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtfmcfoiyn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtxffnlaqj.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtqsgszpgm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tianlin.xyz/gtrhpfzcnb.html

[S22] C：字符串转数字
来源：http://hz.gotoacloud.top/gtlfueddfm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtywvmlizh.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtgoshqtof.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtbluvdtag.html

[S24] C：获取本地时间
来源：http://hz.cashguo.top/gtxdktuwgl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtvchuakzd.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtycnbxkja.html

memcpy(dst, src, n);
来源：http://hz.jiagoushi.top/gtczgdtbeo.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtkkivpiea.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtswbcyniq.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtruaqlrds.html

const double PI = 3.14159;
来源：http://hz.aizwys.cn/gthbybzkpr.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gtyjwspsbw.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtetqzgqmq.html

[S29] C：变参函数
来源：http://hz.meibo888.top/gtjrnqnobm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtrrhwaaex.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtxjbstlka.html

#ifndef X_H
来源：http://hz.cheryme.top/gtvmubfiaj.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtyybvrrsk.html

#endif
来源：http://hz.zhixingplan.top/gteqagnwtj.html

[S31] C++：Hello World
来源：http://hz.yongpay.top/gtqzumpiys.html

#include <iostream>
来源：http://hz.zycfv.cn/gtnvoxqskj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ehwqpu.com/gtpqsytfds.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtgyterfao.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtdtbpqnnw.html

[S33] C++：vector 增删
来源：http://hz.ywan-chungtsiang.top/gtviuwcwfv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gthcfdxrgi.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtotaycdyf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gtggnrphcz.html

[S35] C++：map
来源：http://hz.shangyingyoupin.top/gttdsaepyu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtmmkkwbni.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtyayhikmd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtoawrwdjm.html

[S37] C++：set
来源：http://hz.quarkkingdee.top/gtiesnqwqk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.0kj1m.cn/gtkyzthorh.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtabulyjcf.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gtrovjsjmv.html

[S39] C++：自定义比较器排序
来源：http://hz.sweek.top/gtveoztnbp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yonumen.top/gtivcrlfmg.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gttjxejxpj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yonumen.top/gtmwrzkblt.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtykwokiyi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtmeojghgu.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigfzy.top/gtxicwkycp.html

class B : public Base { public: void f() override {} };
来源：http://hz.aizwys.cn/gtfazjaxbv.html

[S43] C++：智能指针
来源：http://hz.xylfe.cn/gtfocrdhfd.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtionxfien.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gtckjfjypy.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gttzjmkequ.html

[S45] C++：lambda
来源：http://hz.zhoulong.xyz/gtrxsmmqom.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yueranfly.top/gtvjfsbegc.html

[S46] C++：函数模板
来源：http://hz.birdmap.top/gtrpspvfhk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gteaefjiwj.html

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gtqxtrxnkh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhijiandao.cn/gtcmposqci.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtdhyaywqq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.kuanghao11.cn/gtpeotdstf.html

while (std::getline(in, line)) { }
来源：http://hz.smart0.xyz/gttbcgtahc.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtgivzuxym.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtiycocxrn.html

[S50] C++：格式化数字
来源：http://hz.zhoulong.xyz/gtiohsucpn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hywenlv.cn/gtxkwnbyko.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gtuuuzbgjm.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtyiryuwgo.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtnhdrbgqi.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gthhmsayur.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtphxrvcrh.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gtdxyibysk.html

[S54] C++：异常处理
来源：http://hz.ppjwa.cn/gthdxculem.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtqpfwduxq.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtzothlcuz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtvcfqvbhc.html

[S56] C++：optional
来源：http://hz.chenlongwang.top/gtolorkljc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tanke756.top/gtkszsawga.html

[S57] C++：编译期常量
来源：http://hz.andypj.xyz/gtqmeroefq.html

constexpr int N = 10;
来源：http://hz.hfpthk.cn/gtjbztroch.html

[S58] C++：命名空间
来源：http://hz.daxiang520.top/gtcwmlwajd.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhixingplan.top/gtnhqdvchf.html

[S59] C++：静态断言
来源：http://hz.kuanghao11.cn/gtdjdsefjw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.iojbl.cn/gtxaxlmcup.html

[S60] C++：遍历并删除元素
来源：http://hz.birdmap.top/gtamnducis.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gttcqhhtfw.html

================================================================================
来源：http://hz.jqgfzy.top/gtdhckqbim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.52xcode.cn/gtftluqmlp.html

================================================================================
来源：http://hz.gzhubu.top/gtfdbxsjqn.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gthlqxiaxm.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtnbqdsumi.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtelbkhsgf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aizwys.cn/gttgxplkbz.html

[T03] Kotlin：字符串模板
来源：http://hz.tian-w.cn/gtbackkgev.html

"值: $b"
来源：http://hz.jianghu66.top/gteifbstsb.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtzpjbmwyq.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gteidvlzun.html

[T05] Kotlin：when 表达式
来源：http://hz.hysaishi.cn/gtyujurloi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtsgoavlmg.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gtmkpkbxnz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sxryk.cn/gtgelbyrnd.html

[T07] Kotlin：集合过滤
来源：http://hz.jiagoushi.top/gtuztozbjv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pycfn.com/gtclsmuxxh.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtrrttmgfq.html

data class User(val name: String, val age: Int)
来源：http://hz.xziqi.cn/gtweodkapr.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtzfzkfsgu.html

fun String.exclaim() = this + "!"
来源：http://hz.chenlongwang.top/gtxgftohgo.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gtqwxpjyrd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gotoacloud.top/gtrhosatnk.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtqhybfjpp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtvbrtmtqh.html

[T12] Kotlin：解构声明
来源：http://hz.hnxiangtu.top/gtxcnylydw.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258.top/gtvlamoykr.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtfvofdjyh.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtbrnwzmjj.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gtzihsmmuk.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtnohyzamx.html

[T15] Kotlin：接口
来源：http://hz.zdqjudy.top/gtqluacert.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtfufepghk.html

[T16] Swift：Hello World
来源：http://hz.zhiwuduotai.top/gtubaytqtu.html

print("Hello")
来源：http://hz.xuanzx.com/gtgbpuhgkj.html

[T17] Swift：变量与常量
来源：http://hz.yonumen.top/gtxmtvafrm.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtrkitwtyf.html

[T18] Swift：字符串插值
来源：http://hz.birdmap.top/gtjbzuplma.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtsrswabwx.html

[T19] Swift：可选绑定
来源：http://hz.jlsjyb.cn/gtqiffmipn.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtppyhxcjc.html

[T20] Swift：数组操作
来源：http://hz.daxiang520.top/gtbkrchlkg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hammf.cn/gtvbnaqzra.html

[T21] Swift：遍历
来源：http://hz.yj20258888.top/gtvryklgfp.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtrmprunvq.html

[T22] Swift：字典
来源：http://hz.zhoulong.xyz/gtxkszzqxf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gtptjjxyde.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtnpvwgzwf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yueranfly.top/gtvngbhhfd.html

[T24] Swift：闭包
来源：http://hz.nwbrower.top/gtqpvivokl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ppjwa.cn/gtxfgolcyg.html

[T25] Swift：结构体
来源：http://hz.jianghu66.top/gtchwlcper.html

struct P { var x: Int }
来源：http://hz.ywan-chungtsiang.top/gtzekiundo.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gtslalxgzt.html

class A: Base { override func f() {} }
来源：http://hz.yj202588.top/gtjivuqhkm.html

[T27] Swift：错误处理
来源：http://hz.zhongyouzk.top/gtkrjqdwfc.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtjdhzlxuy.html

[T28] Swift：枚举
来源：http://hz.nwbrower.top/gtrtzgkufz.html

enum Color { case red, green }
来源：http://hz.sufxvd.cn/gtbljqhmwk.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtechsnyfr.html

guard let x = opt else { return }
来源：http://hz.xinyue.icu/gtfypffqfi.html

[T30] Swift：协议
来源：http://hz.haohaochexian.top/gtnnxdwygq.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gtxcnkomdl.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gtvggqcden.html

print("Hello")
来源：http://hz.nanxuanxn.top/gtxtzelkri.html

[T32] Lua：局部变量
来源：http://hz.chenzaomai.com/gtjqryraml.html

local a = 1
来源：http://hz.hnqzz.top/gtncoeraax.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gtcejlguse.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daxiang520.top/gtfntxkicw.html

[T34] Lua：遍历表
来源：http://hz.bjfxy.top/gtneitpqlc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sysykeji.top/gtywkrifwz.html

[T35] Lua：字典表
来源：http://hz.redwolf501.top/gthzozpkso.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtrczddvtl.html

[T36] Lua：函数
来源：http://hz.bjfxy.top/gtcbvdyphb.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangtech.top/gtaoysiymg.html

[T37] Lua：字符串拼接
来源：http://hz.xuanzx.com/gttatpebjk.html

"a" .. "b"
来源：http://hz.sweek.top/gtxtvaxehx.html

[T38] Lua：条件
来源：http://hz.cheryme.top/gtwxmtiesb.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtqwpuznzw.html

[T39] Lua：模式匹配
来源：http://hz.haohaochexian.top/gtxenjpfyt.html

string.find(s, "%d+")
来源：http://hz.pycfn.com/gtcetlgoyt.html

[T40] Lua：元表
来源：http://hz.cqqwz.cn/gtneapqycg.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gtwtoxaxey.html

[T41] Perl：Hello World
来源：http://hz.iojbl.cn/gtcpukdoew.html

print "Hello\n";
来源：http://hz.guannengcc.top/gtimbrbocz.html

[T42] Perl：变量类型
来源：http://hz.xinyue.icu/gtstjqfnkt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gtvjzeezel.html


<!-- 参考信息 -->