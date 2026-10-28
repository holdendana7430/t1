代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtlxggfqjw.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gtcpqwmjub.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtmsacawrv.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gtlrgxobub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtlvhbgqiy.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtycssdefa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zdqjudy.top/gtkokwrzdc.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtxtotivhe.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtdnevijmg.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gthmwklmwg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtltbymywk.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtqzmablkw.html

cmd > out.log 2>&1
来源：http://hz.ppjwa.cn/gtlhuvydbd.html

[R40] 追加写日志
来源：http://hz.gogol.net.cn/gtwdzeywgz.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtetftdapd.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtbannsfpv.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtndovvqzj.html

[R42] 输入重定向
来源：http://hz.wangdashe.top/gtysmzpptp.html

wc -l < a.txt
来源：http://hz.sweek.top/gtaoljncjt.html

[R43] 按名字查找文件
来源：http://hz.jqgufenzy.top/gtkregbudj.html

find . -name "*.log" -type f
来源：http://hz.9152youxi.cn/gtfmqknuvk.html

[R44] 按修改时间查找
来源：http://hz.xinyue.icu/gtushujioo.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtetgnzkxi.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtptnzbqsr.html

find . -name "*.tmp" -delete
来源：http://hz.nanxinkj.top/gtqnrqnybw.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtlundohpw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtstuwveap.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gttijgxbto.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigfzy.top/gtdpzvtloy.html

[R48] awk 取指定列
来源：http://hz.daxiang520.top/gttsrnsbgg.html

awk '{print $1, $3}' a.txt
来源：http://hz.fzhhl.top/gtoxenbreb.html

[R49] awk 带条件
来源：http://hz.ehwqpu.com/gtkdmkamfm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtrywknzzs.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtowxjmhan.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtthqxqwuh.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtsqeyrocj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtymqwefhy.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtdcpxwmsn.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtisruespp.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtyehivovd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangkeji.top/gtgdprnfym.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gthpqzwjix.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gthpknehrh.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtnhashwjn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtoytdcykr.html

[R56] 远程拷贝
来源：http://hz.shuidangran.top/gtgxplsbek.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtlhfillzp.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtaozarwez.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtdqbdbdpi.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtqwcqkruj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.birdmap.top/gtshatobrr.html

[R59] 发 POST JSON
来源：http://hz.guowangkeji.top/gtfwpaevov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtyuqsndpf.html

[R60] 只看 HTTP 状态码
来源：http://hz.haohaochexian.top/gtcrawgzzf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.meibo888.top/gtxfztjnnp.html

[R61] 磁盘占用
来源：http://hz.tanke756.top/gtkrmeqqnv.html

df -h;  du -sh *
来源：http://hz.kuanghao11.cn/gthvyvzrvw.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtvpshuctq.html

du -ah . | sort -rh | head -10
来源：http://hz.aizwys.cn/gtlilwqbae.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtgygacshz.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtupufnflo.html

[R64] 结束进程
来源：http://hz.ybcxt.top/gtqkfawelv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtgpjwptuz.html

[R65] 查看端口占用
来源：http://hz.aizwys.cn/gtzadsxdze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtxumtugii.html

[R66] 定时任务
来源：http://hz.yj202588.top/gtznqshnev.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtyrsjcmwz.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtnfxeyphv.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtcupujiih.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gttyajdfje.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtddkdkywh.html

[R69] 生成随机密码
来源：http://hz.redwolf501.top/gtaquzsfek.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtszmkmzoq.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtmwpbhsie.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gtxsmfwgyv.html

[R71] 日期格式化
来源：http://hz.pengpengdd.cyou/gtbnahtmab.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtzdiscfnh.html

[R72] 等待端口就绪
来源：http://hz.fengsongda.top/gtpcjpadja.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtzlurmbkc.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtognheqfp.html

split -l 1000 big.log part_
来源：http://hz.zhengqikj.top/gtzucqjfws.html

[R74] 批量重命名
来源：http://hz.fengsongda.top/gtmzwaqzpw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtalqeieai.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtfjkyvaht.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuanzx.com/gtvgiyjido.html

[R76] 使用临时文件
来源：http://hz.sweek.top/gttpptcuhn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtihrkixvm.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtrmjwahxu.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtagmrcwrw.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtelmeogbe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xylfe.cn/gtzbupboaz.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtcfptmvsu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtgfxptxjs.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtqvmkiuvu.html

time ./run.sh
来源：http://hz.tianlin.xyz/gtndkrilnu.html

================================================================================
来源：http://hz.yj20258.top/gtldlhxsda.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtcrhgrddc.html

================================================================================
来源：http://hz.zhengqikj.top/gtujdrvkuw.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gtnjglfvsu.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gtpdkcnkgj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guannengcc.top/gtfdxastnm.html

[S02] C：变量与格式化输出
来源：http://hz.daxiang520.top/gtxmlprsje.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtrxgfzglt.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtjtrafdwc.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtfgylzsyz.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtdmwagwel.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxinkj.top/gtgiufpbof.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtgzgcuneg.html

strlen(s)
来源：http://hz.jlsjyb.cn/gtqeloxarr.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtwftpcipu.html

strcmp(a, b) == 0
来源：http://hz.guannengcc.top/gtkltpupnu.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtwngiiegf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtokhgyrvq.html

[S08] C：动态内存分配与释放
来源：http://hz.hysaishi.cn/gtkxjwkplr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtjdlxvznh.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtkiounldj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shzxlz.cn/gtbehrxdzv.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtkebylvvq.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtrurakckf.html

[S11] C：逐行读文件
来源：http://hz.daxiang520.top/gtmrcdlgth.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtjatumaxd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtbqxymlqs.html

fclose(f);
来源：http://hz.gotoacloud.top/gtpabsefbp.html

[S12] C：写文件
来源：http://hz.ppjwa.cn/gtvgjbbuik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtdwartnlp.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtyexcfzrv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtllkyfoqd.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtowzbognr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yonumen.top/gtqmqxtyuk.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gttbvzeybh.html

(double) a / b
来源：http://hz.gotoacloud.top/gtwxsjsmys.html

[S16] C：位操作置位
来源：http://hz.shangyingyoupin.top/gtxqgeneik.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtbvfrnuuy.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gtssevqgwa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cdnleiting.top/gtinenddwr.html

[S18] C：命令行参数
来源：http://hz.hnxiangtu.top/gtuggvnsla.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtfleexfpg.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtylmvapey.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtficdccyc.html

[S20] C：二分查找
来源：http://hz.jqgfzy.top/gtqtvurqjk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtaxvxtkbp.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtgsumbwzh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gthvxtizqd.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gttfpcrboi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hywenlv.cn/gtdfemdnom.html

[S23] C：随机数
来源：http://hz.52xcode.cn/gtqyklyjod.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtclyedlmy.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtwxldmgjq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtjountngc.html

[S25] C：内存拷贝
来源：http://hz.yj20258888.top/gtkzwhtdyx.html

memcpy(dst, src, n);
来源：http://hz.ivvv.top/gtsisjyjor.html

[S26] C：内存清零
来源：http://hz.havefunace.top/gtgovqqaqq.html

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gtxnxarmuk.html

[S27] C：定义常量
来源：http://hz.jinyuanbaomall.cn/gtdczekoww.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtyivwtruh.html

[S28] C：静态变量
来源：http://hz.quarkkingdee.top/gtuanysfgo.html

static int counter = 0;
来源：http://hz.yj20258888.top/gttwubzyab.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtrkdzffqm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sysykeji.top/gtnlwcxiln.html

[S30] C：头文件保护
来源：http://hz.shzxlz.cn/gttaotlxox.html

#ifndef X_H
来源：http://hz.hnqzz.top/gtxxsskbif.html

#define X_H
来源：http://hz.jianghu66.top/gtaerxozub.html

#endif
来源：http://hz.xuetiantiany.cn/gtzuolrdmt.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtpprmvxfi.html

#include <iostream>
来源：http://hz.guannengcc.top/gtbhyrgjsk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.redwolf501.top/gtyspompmu.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gtzqfybclo.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gtkoxwvkon.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtpjtsdjuy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.c1oappe.top/gtdqeentzw.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtiqkcwtgt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gtqmpzrxqo.html

[S35] C++：map
来源：http://hz.yueranfly.top/gtbyflhpdr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtuofzkybn.html

[S36] C++：unordered_map
来源：http://hz.gaohongyu789.top/gtmopnwxlp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtaqsatzwb.html

[S37] C++：set
来源：http://hz.jyoumei.cn/gtmcoxsnxl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gogol.net.cn/gtmsysjhfv.html

[S38] C++：排序
来源：http://hz.chenzaomai.com/gtprgixzbs.html

std::sort(v.begin(), v.end());
来源：http://hz.cqqwz.cn/gtrlzkmbyk.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtgyblzjzi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ivvv.top/gtrcrozthf.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtckgudlih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gtgjjefndd.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gthmmamghp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.316326.xyz/gtejlcpesg.html

[S42] C++：继承与虚函数
来源：http://hz.yonumen.top/gtpkdtkfay.html

class B : public Base { public: void f() override {} };
来源：http://hz.quarkkingdee.top/gtkfwoengh.html

[S43] C++：智能指针
来源：http://hz.yj20258.top/gtxdvtafhg.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gtftcyhroy.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtlyzrvwxp.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gthqrxdgbn.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtskrmrwwh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtkrttzmlp.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtncqpdcnx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gthsaiiozc.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtpokfkvco.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ehwqpu.com/gtsndzlxww.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtlbzxtqzy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtrafmtqgb.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtddvzmaho.html

[S49] C++：写文件
来源：http://hz.xinyue.icu/gtohpnokgq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtkmvvvqto.html

[S50] C++：格式化数字
来源：http://hz.tianlin.xyz/gthynyveez.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fengsongda.top/gtvvwnvvte.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtfommxtem.html

static_cast<double>(a) / b
来源：http://hz.zhixingplan.top/gtrdntjuaz.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gtoktznltk.html

int size() const noexcept { return n_; }
来源：http://hz.meibo888.top/gtcdeqxkbj.html

[S53] C++：移动语义
来源：http://hz.jinqigufen.top/gtpnzjlosj.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtrwxuallh.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gttpevlhla.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenzaomai.com/gtsvybgwus.html

[S55] C++：结构化绑定
来源：http://hz.tianlin.xyz/gtcwhqplto.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gtmfdcrwci.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gtwnrbaugf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sweek.top/gteedhzauy.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtyjcsoakb.html

constexpr int N = 10;
来源：http://hz.kuanghao11.cn/gttgyefgis.html

[S58] C++：命名空间
来源：http://hz.aizwys.cn/gtaivytjzs.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtkdruuxfh.html

[S59] C++：静态断言
来源：http://hz.snrcjt.cn/gthhjnzmwo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuxming.cn/gtzvzwgilc.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtswxsldid.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtcviyluok.html

================================================================================
来源：http://hz.cqqwz.cn/gtprtwtcwm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daria6918.cn/gtxviosjrh.html

================================================================================
来源：http://hz.tanke756.top/gtuomhgtli.html

[T01] Kotlin：Hello World
来源：http://hz.sxryk.cn/gtxejjhrll.html

println("Hello")
来源：http://hz.hammf.cn/gttccileuq.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gtsnwfeund.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cucudq.cn/gtdwoeqwmo.html

[T03] Kotlin：字符串模板
来源：http://hz.hywenlv.cn/gtomnybqcc.html

"值: $b"
来源：http://hz.bjfxy.top/gtovfdidaj.html

[T04] Kotlin：空安全
来源：http://hz.snrcjt.cn/gtmxtsjzpz.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtshmggdha.html

[T05] Kotlin：when 表达式
来源：http://hz.dianchejie.cn/gtwmhmmtfc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hongshengwenyu.top/gtvxymbjdy.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gtrgpcuzmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.snrcjt.cn/gtwvcrromz.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtyttnyvaf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hysaishi.cn/gtawuoynxx.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtmwjuvfwh.html

data class User(val name: String, val age: Int)
来源：http://hz.c1oappe.top/gtfucxdfjd.html

[T09] Kotlin：扩展函数
来源：http://hz.chenzaomai.com/gtdrxtotja.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtkflzffdn.html

[T10] Kotlin：默认参数
来源：http://hz.hysaishi.cn/gtbmbeijtu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ybcxt.top/gtbcxnxxmk.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtlgwrqvuh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.9152youxi.cn/gtbawugjuc.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtyxljzsqa.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxuanxn.top/gtcqbdhoak.html

[T13] Kotlin：只读 Map
来源：http://hz.feifeiyinyue.top/gtrwckyhrq.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gtanqjglps.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtviqskcye.html

for (i in 1..10) println(i)
来源：http://hz.9152youxi.cn/gtfemnkhgo.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtntzlhdzo.html

interface Shape { fun area(): Double }
来源：http://hz.cashguo.top/gtnrhiufuq.html

[T16] Swift：Hello World
来源：http://hz.ehwqpu.com/gtlizmuznn.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtahqkkitk.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtxpwqtbbz.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtkwzgvwkh.html

[T18] Swift：字符串插值
来源：http://hz.zhiwuduotai.top/gtqvkgjylq.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gtwoqedwfd.html

[T19] Swift：可选绑定
来源：http://hz.vqdsnc.cn/gtpbazlzdw.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtgndhizlq.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gtiyopxtys.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.kuanghao11.cn/gtnrhatmzg.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtzdmegbqk.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtioogzaqm.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtpbfazwgj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtfeiimiuh.html

[T23] Swift：函数
来源：http://hz.havefunace.top/gtmciqxvdk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuanzhike.top/gtpiudbteu.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtzctxctrd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.pycfn.com/gtihrgxpjc.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtjtpetbaw.html

struct P { var x: Int }
来源：http://hz.cashguo.top/gtmryjtbqr.html

[T26] Swift：类与重写
来源：http://hz.xuetiantiany.cn/gtbziksokp.html

class A: Base { override func f() {} }
来源：http://hz.nanxinkj.top/gthnpctvui.html

[T27] Swift：错误处理
来源：http://hz.pengpengdd.cyou/gtaqfazdrb.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gtadtfsiih.html

[T28] Swift：枚举
来源：http://hz.chenlongwang.top/gtnbbkmhwi.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtzwnrqbwn.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtwfpvjezz.html

guard let x = opt else { return }
来源：http://hz.aibaodan.cn/gtajfqqcqd.html

[T30] Swift：协议
来源：http://hz.yj20258.top/gtmyyoaywp.html

protocol Shape { func area() -> Double }
来源：http://hz.fzhhl.top/gtedfdylmi.html

[T31] Lua：Hello World
来源：http://hz.cucudq.cn/gtsxsdsbon.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtthzwgndo.html

[T32] Lua：局部变量
来源：http://hz.chenzaomai.com/gtaejntcac.html

local a = 1
来源：http://hz.zhengqikj.top/gtvkccsszp.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtagtnlzib.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shzxlz.cn/gtmdmqjmbi.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtyhczmqcg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhengqikj.top/gtjkamvvqa.html

[T35] Lua：字典表
来源：http://hz.iojbl.cn/gtzmcmacqr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pycfn.com/gtfbgwhkdx.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtctmqcolo.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtyldtcrwn.html


<!-- 参考信息 -->