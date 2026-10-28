代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtfisagbzv.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtrfuzhgyo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hysaishi.cn/gtoinqeogf.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gtcquhevdd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtzzpcohxz.html

[R34] 退出时清理
来源：http://hz.hnxiangtu.top/gtwjipcoyx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtwvnlwyuk.html

[R35] 后台执行并等待
来源：http://hz.pengpengdd.cyou/gtukhuipha.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtfvojgiit.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtihmluqdv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtyeqdulac.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtwbyqftdj.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtvcbkqbga.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gtndnaiqgp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cdnleiting.top/gtkgwgjham.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtknobgutz.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtjqwzuxcb.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtzhnduacg.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gthophfecf.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtskrbkadh.html

cmd >/dev/null 2>&1
来源：http://hz.xylfe.cn/gtwuppoeyv.html

[R42] 输入重定向
来源：http://hz.ivvv.top/gtxrtavpjy.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtvhevpkas.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtrmapldbs.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtujhetfhb.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gtboghrhqf.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtpdrfquul.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtomkgcudc.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtcqxtixkr.html

[R46] 递归替换文件内容
来源：http://hz.jinqigufen.top/gtphhtvwak.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtfdfqljql.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtfaezqhse.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtzaugflmx.html

[R48] awk 取指定列
来源：http://hz.guowangkeji.top/gtxzcvqwhn.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtghnvubng.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gthcjuwfww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.vqdsnc.cn/gtxrrlbwlk.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtjxpmqaic.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sweek.top/gtbabqvlee.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtktbhajsr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.vqdsnc.cn/gtjfgzagqc.html

[R52] 统计行数
来源：http://hz.sweek.top/gtyluzrmgy.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtzgtdwylq.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtjutufqxn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gaohongyu789.top/gtjwhuwybs.html

[R54] 比较两个文件
来源：http://hz.wangshuangyany.cn/gtfyymyxap.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtiocnnkav.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtkioostmt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jianghu66.top/gtjqgfcfhp.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtkghaxejo.html

scp file user@host:/path/
来源：http://hz.jinghuilouyu.cn/gtbgkiybde.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtknfsoqar.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gtwyyylamd.html

[R58] 下载文件
来源：http://hz.xingfuxueyuan.xyz/gtcphkyrvr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gthsmmzzyx.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtcvombxme.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtktxlkiph.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuxming.cn/gteorgmviy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtxdjzfnhs.html

[R61] 磁盘占用
来源：http://hz.cdnleiting.top/gtkxpdsfqq.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtjbmcqcuf.html

[R62] 找最占空间的文件
来源：http://hz.meibo888.top/gtboyegtuy.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtnfbchlkp.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtknrrkvwj.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtadgpdbyl.html

[R64] 结束进程
来源：http://hz.gogol.net.cn/gtzgmhgkep.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtbvopbpiq.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtsygmekjr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtyqitlknw.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtdvtywtwx.html

crontab -e;  crontab -l
来源：http://hz.yuxming.cn/gtzhmbuvki.html

[R67] 生成随机十六进制串
来源：http://hz.yongpay.top/gtbiyatlvn.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtxfcxfbnp.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtxmkcsndi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gtibprgwjo.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtumslsjkh.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtkcbbidvk.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtfefuppke.html

date +%s;  date -d @1700000000
来源：http://hz.fzhhl.top/gtkdqajzfz.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtgwsmbgwx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtxuzyagsp.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtqrbmwqms.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtaljysjra.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtxdmulkpt.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtnhtzciqr.html

[R74] 批量重命名
来源：http://hz.zhiwuduotai.top/gtrmjiqzsu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtldsxhkic.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtwzmthxup.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtcgmkoxhm.html

[R76] 使用临时文件
来源：http://hz.dianchejie.cn/gtfmqsjhiy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtyrjlwyir.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtvipzpmex.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtlbfdzvbs.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtzvkwfzbi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtirikonmy.html

[R79] 解析命令行选项
来源：http://hz.0kj1m.cn/gtjjmjgjgj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtphczwygg.html

[R80] 查看脚本执行耗时
来源：http://hz.pycfn.com/gtxcehefyd.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtqtwrjplf.html

================================================================================
来源：http://hz.guowangkeji.top/gtrrviajus.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtlpshuycg.html

================================================================================
来源：http://hz.bjfxy.top/gtkdremvos.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtiaxlhjbp.html

#include <stdio.h>
来源：http://hz.cheryme.top/gttheoonrq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tianlin.xyz/gtepufeghe.html

[S02] C：变量与格式化输出
来源：http://hz.andypj.xyz/gtunlwkffv.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtmnexkglu.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtvwlescch.html

int x; scanf("%d", &x);
来源：http://hz.hnqzz.top/gtrthbzkig.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtgjyrqbfg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtqvcetyym.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtkohxxjpx.html

strlen(s)
来源：http://hz.chenjidiqi.icu/gtmpqxzfzv.html

[S06] C：字符串比较
来源：http://hz.hongshengwenyu.top/gtedczseyp.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtfkowjytv.html

[S07] C：数组遍历求和
来源：http://hz.jinyuanbaomall.cn/gtprwdhufa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtxxyxqqvn.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gthsfygpzv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtrtbcbepi.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtxljteqml.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigfzy.top/gtrqtvnder.html

[S10] C：指针与解引用
来源：http://hz.sysykeji.top/gtcixxfmti.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtovcqujbw.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtjcfvhamt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtewlgiitu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.svipenyu.cn/gtjirkfwgu.html

fclose(f);
来源：http://hz.tanke756.top/gtsevflakf.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtpsocgodq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.c1oappe.top/gtvvdyllch.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gttukhyovu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtoefnxxqa.html

[S14] C：枚举
来源：http://hz.ywan-chungtsiang.top/gtfioyzhfc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gteddiqmrv.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtezippgqa.html

(double) a / b
来源：http://hz.aibaodan.cn/gtptwnjvox.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtzqabbudx.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gtdlmjevgn.html

[S17] C：安全拼接字符串
来源：http://hz.haohaochexian.top/gtpkehjebr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sysykeji.top/gtqlvlymyv.html

[S18] C：命令行参数
来源：http://hz.gotoacloud.top/gtcakbjtud.html

int main(int argc, char **argv)
来源：http://hz.haohaochexian.top/gtoawrdqgg.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtsdvaxzpw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtwcdtpwki.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtvfndwaiu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gthfyailfm.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtmpnbnsam.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtcdvteavb.html

[S22] C：字符串转数字
来源：http://hz.snrcjt.cn/gtkfyiamum.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yanxiufei.cn/gtmkkjstba.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtzgapbxjm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.iojbl.cn/gtchhryvpc.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtoatcynpx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangkeji.top/gtjnuswbnk.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtljkxjtlm.html

memcpy(dst, src, n);
来源：http://hz.ywan-chungtsiang.top/gtuzdmsrwa.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtmrbrhcnf.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtagknudcx.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gthyqcgtel.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtbuijkznj.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtwjdehcyn.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtoujufvec.html

[S29] C：变参函数
来源：http://hz.hywenlv.cn/gtpkipioqu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtabyytbro.html

[S30] C：头文件保护
来源：http://hz.ivvv.top/gthgdlzrbg.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtgdufvtbh.html

#define X_H
来源：http://hz.316326.xyz/gtwuggwpmq.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtwldozkdg.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtmpjlylej.html

#include <iostream>
来源：http://hz.jyoumei.cn/gtuescoodv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jlsjyb.cn/gteknemtas.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtpyuskkum.html

std::string s = "hi";  s += "!";
来源：http://hz.birdmap.top/gtgkdmsjpj.html

[S33] C++：vector 增删
来源：http://hz.zhongyouzk.top/gtkqwakpgh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cqqwz.cn/gtufqbwzlj.html

[S34] C++：遍历 vector
来源：http://hz.yonumen.top/gtlfmgxtzp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtxvyveksb.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtiyuqkkyt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtdwrchsxd.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtrcjbcjor.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtyfrovkei.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtsldmqocu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.haohaochexian.top/gtlpmgqytp.html

[S38] C++：排序
来源：http://hz.shanyushiyangkeji.top/gtqjptubvp.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtjdcsxaze.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtvsvqifok.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtidcrbljd.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gthiafsgli.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtaykdvfog.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtlfqylxfd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gtyxxxgjpp.html

[S42] C++：继承与虚函数
来源：http://hz.hammf.cn/gtmsoarghl.html

class B : public Base { public: void f() override {} };
来源：http://hz.guowangkeji.top/gtonjkloax.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtppfsgpbo.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtuioecsfu.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtxhehvrjb.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtnibgzqay.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtnovlxqxu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.vqdsnc.cn/gtxhiuxtcj.html

[S46] C++：函数模板
来源：http://hz.hongshengwenyu.top/gtjygovqeu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtsdizrbxc.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtjgcsxkcm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtrazoamkb.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtgudwonwi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.0kj1m.cn/gtwvsioidj.html

while (std::getline(in, line)) { }
来源：http://hz.redwolf501.top/gtehpguzke.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtlojzdmqk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gtqllnejem.html

[S50] C++：格式化数字
来源：http://hz.guannengcc.top/gtrusodvtl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cashguo.top/gtrdrozwab.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtmoxwzoaq.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtjmaijsoo.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtouqmemfv.html

int size() const noexcept { return n_; }
来源：http://hz.zhixingplan.top/gtvcfljfqp.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtivuetlpw.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtmipilwwv.html

[S54] C++：异常处理
来源：http://hz.jinyuanbaomall.cn/gtoywxdafp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtqzzuvrzi.html

[S55] C++：结构化绑定
来源：http://hz.yuanzhike.top/gtsoomazec.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhoulong.xyz/gtqixsykms.html

[S56] C++：optional
来源：http://hz.havefunace.top/gteuwfpfjw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtaugtzbhb.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtaryztbxr.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gtjreopvli.html

[S58] C++：命名空间
来源：http://hz.cheryme.top/gtebsfhjel.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gtodmyqqlo.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtcfnakdzl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtzdwieflq.html

[S60] C++：遍历并删除元素
来源：http://hz.ivvv.top/gtqhqavlas.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnxiangtu.top/gtnzxgiaiv.html

================================================================================
来源：http://hz.yvedp.cn/gtmczxanhj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtlltwthkj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsquwczlm.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtnjvecjhq.html

println("Hello")
来源：http://hz.cashguo.top/gtbkgprdmc.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtoqxbfibj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtfrusgguc.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtajqhhtnr.html

"值: $b"
来源：http://hz.yongpay.top/gtuvovlurm.html

[T04] Kotlin：空安全
来源：http://hz.zhoulong.xyz/gtiwmlaubt.html

val n: String? = null;  n?.length
来源：http://hz.yj202588.top/gtnxsmxxxz.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gttdcnqxtn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sysykeji.top/gtsljqpnru.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtrixxsqlt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtsmltuajd.html

[T07] Kotlin：集合过滤
来源：http://hz.sweek.top/gtgduswaqp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guannengcc.top/gtolixqoko.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtqmdmtllf.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gtbcpueslr.html

[T09] Kotlin：扩展函数
来源：http://hz.wangdashe.top/gtgdcxlliz.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtogzifpni.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtarhjjftg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gthlunytwc.html

[T11] Kotlin：协程
来源：http://hz.jqgufenzy.top/gtxztevkjd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxuanxn.top/gtvhvkdkqe.html

[T12] Kotlin：解构声明
来源：http://hz.hfpthk.cn/gtziakimww.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtvyapbglo.html

[T13] Kotlin：只读 Map
来源：http://hz.hnxiangtu.top/gtwsmrgrnl.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gtjlmwaohz.html

[T14] Kotlin：循环
来源：http://hz.sysykeji.top/gtojozolhy.html

for (i in 1..10) println(i)
来源：http://hz.zhixingplan.top/gtyktnmtbw.html

[T15] Kotlin：接口
来源：http://hz.daxiang520.top/gtddendkfv.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtqvuyxqes.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtqzvoopsk.html

print("Hello")
来源：http://hz.yuxming.cn/gtkxpjezvp.html

[T17] Swift：变量与常量
来源：http://hz.zhijiandao.cn/gtkusxguyi.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtkaqixjjq.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtzxsdnuym.html

"值: \(b)"
来源：http://hz.ehwqpu.com/gttjcjmzom.html

[T19] Swift：可选绑定
来源：http://hz.hnqzz.top/gtnaqodqux.html

if let n = opt { print(n) }
来源：http://hz.dianchejie.cn/gtyvckpeie.html

[T20] Swift：数组操作
来源：http://hz.andypj.xyz/gtfsjcevgc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtrxkusllq.html

[T21] Swift：遍历
来源：http://hz.aibaodan.cn/gtcjmpuzrt.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtdyfubzwx.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gtpmizfgdr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dianchejie.cn/gtwuqtczol.html

[T23] Swift：函数
来源：http://hz.shzxlz.cn/gtrdkzhfru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtgoxduvgs.html

[T24] Swift：闭包
来源：http://hz.meibo888.top/gtfwdktphb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gtxrswspal.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtxycwhhts.html

struct P { var x: Int }
来源：http://hz.zdqjudy.top/gtmmcqyiys.html

[T26] Swift：类与重写
来源：http://hz.redwolf501.top/gtpiyxuvij.html

class A: Base { override func f() {} }
来源：http://hz.316326.xyz/gtpokwqalc.html

[T27] Swift：错误处理
来源：http://hz.c1oappe.top/gtpzjtawwn.html

do { try f() } catch { print(error) }
来源：http://hz.jyoumei.cn/gtesrjiehh.html

[T28] Swift：枚举
来源：http://hz.daria6918.cn/gtbgutnsfv.html

enum Color { case red, green }
来源：http://hz.nanxinkj.top/gtassomraz.html

[T29] Swift：guard 提前返回
来源：http://hz.meibo888.top/gtdynpqkwx.html

guard let x = opt else { return }
来源：http://hz.daria6918.cn/gtamsvtxzq.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtpvmqoxgj.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gtcurxovvh.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtetybelll.html

print("Hello")
来源：http://hz.ydzc1.top/gtezhqtkwp.html

[T32] Lua：局部变量
来源：http://hz.cashguo.top/gtqkcnkuww.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gtkqvytpkc.html

[T33] Lua：表（数组）
来源：http://hz.smart0.xyz/gtmgogiute.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtsaivozui.html

[T34] Lua：遍历表
来源：http://hz.jianghu66.top/gtwylzqcmv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtuilvuvmw.html


<!-- 参考信息 -->